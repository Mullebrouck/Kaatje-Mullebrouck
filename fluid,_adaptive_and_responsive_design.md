# Fluid, Adaptive and Responsive Design

- standard phone is height: 420px and width: 320px
- standard tablet width : 768px

#Fluid Layout

- Fluid layout = layout that scales
- Fixed layout = layout that is static

**Don't set `fixed widths` on elements that do not need it**

###Converting `pixels` into `ems`

- default font-size browser = 16px
- setting `body{ font-size: 62.5% };` --> is 1em = 10px
- if you don't reset `body{ font-size: };` use the 16px as `content`

`Target / content = Result`
- Target = target font-size
- Content = Font-sie containing element

Convert tool: http://responsv.com/flexible-math/

###Fluid site

- fluid grid
- relative values should be in `%` instead of `px`

Using Formula:
`Target / content = Result`

**Flexible Margins**
- content = width of elements container

#Adaptive Design

= designing for specific context

4 Design keys:
- user?
- how they will use the site?
- context (device)
- content (how will it adapt?)

###Adaptive Markup

example: 
- header
- menu
- about

###Break Points

- where design breaks down
- in adaptive design will be height and width of target viewport

###Media Queries

```html
<link rel="stylesheet" href="global.css" media="all" />
<link rel="stylesheet" href="main.css" media="screen" />
<link rel="stylesheet" href="paper.css" media="print" />
```
with standard phone height:
```css
@media screen and (max-width: 320px) {
  body {
    font-size: 100%;
  }
}
@media screen and (min-width: 1024px) {
  body {
    font-size: 100%;
  }
}
```
- screen = media type
- max-width = query

**Place your queries at bottom of your stylesheet**

- to stack two blocks of content that would be next to each other on the desktop, we will inherit them: 
```css
.box {
  ...
  ...
  width: inherit;
}
.BLOCK1 {
  float: none;
}
.BLOCK2 {
  float:none;
}
```

#Responsive Design

= content defines break point

```css
@media screen and (max-width: BREAKPOINT px) {
 ADJUSTED CSS STYLES
}
```

example with tablet:

```css
@media screen and (max-width: 768px) {
   .box {
      ...
      ...
      width: inherit; --> so boxes go on top of each other
   }
   .BLOCK1 {
     float: none;
   }
   .BLOCK2 {
     float:none;
   }
}
```

#Responsive Media

###Responsive Images

- save image out larger and use `max-width:100%` so you can get full resolution

```css
img {
  max-width: 100%;
}
about img {
  width: 29%;
}
```
But also for following media:
- `img{ max-width:100%; }`
- `embed{ max-width:100%; }`
- `object{ max-width:100%; }`
- `video{ max-width:100%; }`

###Retina Images

Retina images = 1.5-2 times the pixel density (Use Media queries to target them)

```css
@media 
only screen and (-webkit-min-device-pixel-ratio: 1.5),
only screen and (min-device-pixel-ratio: 1.5){
/*Styles*/
}
```
**Saving images for retina**

Example: 
- NAME.png = 200px
- NAME@2x.png = 400px --> Adding `@2x` to your name

**Show to add**

Example
logo.png = 12px by 16px
logo@2x.png = 24px by 32px
```css
/*ORIGINAL CSS*/
.logo {
  background-image: url(images/logo.png) no-repeat;
}
```
```css
/*ADDING MEDIA QUERY*/
@media 
only screen and (-webkit-min-device-pixel-ratio: 1.5),
only screen and (min-device-pixel-ratio: 1.5){
  .logo{
    bakground-image: url(images/logo@2x.png) no-repeat;
    -webkit-background-size: 12px 16px;
    background-size: 12px 16px; (needs to be equal to original image)
  }
}
```

###Picturefill

- creates `<picture>` element
- need to put `picturefill.js` into <head>

```html
<picture alt="ADD TEXT">

  <!--smallest size first - no @media qualifier-->
  <source src="content-image.jpeg" />

  <!--larger size - send to viewport 800px wide and up-->
  <source src="content-image-large.jpeg" media="(min-width:800px)" />

  <!--fallback content for non-js or non-media-query-supporting-browsers-->
  <noscript>
    <img src="content-image.jpeg" alt="ADD TEXT"/>
  </noscript>

</picture>
```







