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
