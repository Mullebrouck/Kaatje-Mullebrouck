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