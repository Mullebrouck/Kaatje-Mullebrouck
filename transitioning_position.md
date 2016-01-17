# Transitioning Position


##Transitioning in Hidden Button Content

Original Button

```html
    <a href="#" class="container">
     Text for Button
    </a>
```

### Create 2 inner divs

Holds current and additional information shown on button hover:

```html
<a href="#" class="container">
  <div class="content red">Red</div>
  <div class="content yellow">Yellow</div>
</a>
    
```

### Create transition between hover and state

```css
.container {
/*   overflow: hidden; */
  height: 30px;
  background-color: green;
  display: inline-block;
  width: 120px;
  background-color: green;
  position: relative;
}

.content {
    position: absolute;
    transition: top 0.3s;
    line-height: 30px;
    width: 120px;
    text-align: center;
}

.red {
  top: 0px;
  background-color: red;
}

.container:hover .red {
  top: -30px;
}

.yellow {
  top: 30px;
  background-color: yellow;
}
.container:hover .yellow {
  top: 0px;
}
```
[](codepen://Kaatje/GoMXwd)





