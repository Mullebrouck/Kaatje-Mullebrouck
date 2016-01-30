# Navigation

- Use unordered list for navigation
- configuring navigation with a list, provides accessibility. 
- Try not to use `<br>`

##Vertical Navigation with unordered list

1. Write the HTML
2. Configure CSS
3. Remove Underline with CSS

**Write the HTML**

```html
<ul>
    <li><a href="index.html">Home</a></li>
    <li><a href="menu.html">Menu</a></li>
    <li><a href="product.html">Product</a></li>
    <li><a href="Contact.html">Contact</a></li>
</ul>
```

**Configure CSS**

```css
nav ul {
    list-style-type: none; //takes list markers away
}
```

**Remove Underline with CSS**

```css
nav ul {
    list-style-type: none; 
}
nav a {
    text-decoration: none; //takes the underline away
}
```
___

##Horizontal Navigation with unordered list

1. Write HTML
2. Configure with CSS


