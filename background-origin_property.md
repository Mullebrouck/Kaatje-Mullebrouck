## Background-Origin Property

= **positions the background image using the values:**

- content-box (positions relative to area)
- padding-box (default; position relative to padding area)
- border-box (position relative to border area)

![](http://www.w3schools.com/css/box-model.gif)


Example:
```css
.test {
    background-image: url(myimage.jpg);
    background-clip: content-box;
    background-repeat: no-repeat;
    background-position: right top;
    width: 400px;
    padding: 20px;
    margin-bottom: 10px;
    border: 1px dashed #000;
}
```
> No effect when background-image property is set to fixed!