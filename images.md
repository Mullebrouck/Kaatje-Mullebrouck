# Images

# Content Images
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


# Layout Images  
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

# User Interface Images
- help to understand the content of the page

