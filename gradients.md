# Gradients

= **Smooth Blending of shades from one color to another**


###Linear Gradient Syntax

`linear-gradient` in `background-image` propert:
- to bottom
- to top
- to left
- to right

Example:

```css
background-image: linear-gradient(to bottom, start-color, end-color);
```

___
###Gradients and Progressive Enchancement

Make sure you create a fallback `background-image` or `bachround-color` in case browser does not support this. 

---

###Configuring Gradients

Insert webkits: 

- -webkit-linear-gradient (Safari)
- `filter` instead of `linear-gradient` (IE9-)
- `linear-gradient` (W3C Syntax)

Example

```css
body {
    background-color: #8FA5CE;
    background-image: -webkit-linear-gradient(#FFFFFF, #8FA5CE);
    filter: progid:DXImageTransfrom.microsoft.gradient(startColorstr=#FFFFFFFF; endColorstr=#FF8FA5CE);
    background-image: linear-gradient( to bottom, #FFFFFF, #8FA5CE); 
}
```

