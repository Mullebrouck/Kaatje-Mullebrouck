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