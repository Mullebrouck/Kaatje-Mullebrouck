## Background-Clip Property

= **confines the display of background image with the values:** 

- content-box (display area behind content)
- padding-box (display area behind content and padding)
- border-box (display area behind content, padding and border)

![](http://www.w3schools.com/css/box-model.gif)


Example:
```css
.test {
    background-image: url(myimage.jpg);
    background-clip: content-box;
    width: 400px;
    padding: 20px;
    margin-bottom: 10px;
    border: 1px dashed #000;
}
```
