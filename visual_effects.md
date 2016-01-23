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

---

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

___

## Background-Size Property

= **used to resize or scale background-image with values:**

- Both percentage values for weight and height
- Both pixel values for weight and height
- cover (completely cover area --> Looks at smallest size to cover)
- contain (completely one area --> Looks at biggest size to cover)






