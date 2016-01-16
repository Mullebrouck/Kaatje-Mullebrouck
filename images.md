# Images

# content images
- Actual images on page that are necessary
- display logo/site
(put them in one folder)

```html
<img src="LOCATION IMAGE" alt="PUT HERE DESCRIPTION OF IMAGE" >
```

* Always "inline" level (_Can't be centered with text-align_)

**To center:**

```css
display: block;
margin: 0 auto 0 auto;
```

**When added to list:**

  remove bullet points: 

```css
list-style-type: none;
```

remove padding: 

```css
padding: 0;
```


# layout images  
- part of background to make layout nicer
- only added in CSS

```css
background-color: (_needs to be set in case image does not load_)
background-image: url(PATH TO IMAGE FILE);
background-position: *first word*: top,center or bottom *Second word*: left, center or right;
background-repeat: repeat;
```

**other values:**

- repeat-x: tile image horizontally
- repeat-y: tile image vertically
- no-repeat: don't repeat anything


### Or put background in one line:

```css
background: COLOR IMAGE POSITION REPEAT;
```

**Writing on top of background images**

Create empty div container that contains background and put text tags in it. 

  + Create div tag with class in HTML

```html
<div class="NAME OF CLASS">
  <h1,h2,h3,...> TEXT ON TOP OF BACKGROUND </h1,...>
<\div>
```

  + Adjust CSS

```css
.NAME OF CLASS {
  width: ;
  height: ;
  background: COLOR IMAGE POSITION REPEAT;
}
```


# Floating images
- used when you want to put text and images next to each other

* put content you want to have together in a `<li>`

example: 

```html
<ul class="NAME OF CLASS">
   <li>
       <img src="....">
       <h3><a href=".....">CONTENT</a></h3>
       <p> </p>
   </li>
</ul>
```

```css
.NAME OF CLASS img {
  float: left, right or center;
  padding-right: 10px; (to make sure you have some space between image and text)
}
```

# user interface images
- help to understand the content of the page

# Cropping Images

**Overflow Crop Method**

add crop class

example:
```html
<ul class="NAME OF CLASS">
   <li class="crop">
       <img src="....">
       <h3><a href=".....">CONTENT</a></h3>
       <p> </p>
   </li>
</ul>
```
```css
.crop {
  height: 300px;
  width: 400px;
  overflow: hidden;
}
```
+ landscape images: 
```css
.crop img {
  height: auto;
  width: 400px;
}
```
+ portrait images: 
```css
.crop img {
  height: 300px;
  width: auto;
}
```

# Replacement images

Adding descriptive text to image replacement elements. (like logo with text)

```html
<a href="#" class="CLASSNAME"> Place text from image in here </a>
```
To let text disappear add `text-indent` in css
```css
.logo {
  background: url(IMAGE);
  display: block;
  width: 100px;
  height: 100px;
  text-indent: -9999px;
}
```

# Sprites

```html
<a href="#" class="CLASSNAME"> Place text from image in here </a>
```
To let text disappear add `text-indent` in css
```css
.CLASSNAME {
  background: url(IMAGE);
  display: block;
  width: 100px;
  height: 100px;
  text-indent: -9999px;
}
``` 
When adding `:hover, :focus` problems will occur
```css
.logo:hover, .logo: focus{
}
``` 
Need to combine the images in one file and use `background-position`
```css
.logo:hover, .logo: focus{
  background-position: 0 -100px; (depending what height of first image is)
}
``` 

**Multiple states and images**

example:
```html
<ul class="CLASSNAME"> 
  <li><a href="#" class="CLASSNAME1"> Place text from image1 in here </a></li>
  <li><a href="#" class="CLASSNAME2"> Place text from image2 in here </a></li>
</ul>
```
```css
li {
  float: left;
  margin-right: 20px;
}
```

```css
.CLASSNAME1, .CLASSNAME2 {
  background: url(IMAGE);
  display: block;
  width: 100px;
  height: 100px;
  text-indent: -9999px;
}
.CLASSNAME2 {
  background-position: -100px 0;
}
.CLASSNAME1:hover, CLASSNAME1:focus;
  background-position: 0 -100px;
}
.CLASSNAME2:hover, CLASSNAME2:focus;
  background-position: -100px -100px;
}
```