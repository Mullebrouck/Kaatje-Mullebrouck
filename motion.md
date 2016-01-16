# Motion

Use Vendor Prefixes:
* to check browser support for prefixes: [caniuse.com](caniuse.com)

```css
.button{
 -webkit-transition: background-color .4s; (safari, chrome)
 -moz-transition: background-color .4s; (firefox)
 -ms-transition: background-color .4s; (internet explorer)
 -o-transition: background-color .4s;
 -transition: background-color .4s;
}
```
##Transitioning Background

Adding 
* `transition: <property> <duration>;`
* `transition: all <duration>;` --> Multiple properties with same speed

```html
<a href='#' class='button'>
Click here
</a>
```
```css
.button {
 background-color: #ffffff;
 transition: background-color 0.5s;
}
.button:hover {
 background-color: #3456dd;
}