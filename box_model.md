# Box Model

- content = `width`
- padding = `padding`
- border = `border`
- margin = `margin`
- Box width = `content width + adding width + border width;`
 

---



### Border Properties

`border` property default = 0 (does not display)
    
    border-color
    border- width
    border-style
    border-top
    border-bottom
    border-right
    border-left
    
`border-style` formatting options:

    inset
    outset
    double
    groove
    ridge
    solid
    dashed

**Example:**
```css
.dashedborder {
    border-width: 3px;
    border-style: dashed;
    border-color: #000033;
}
```
shorthand Notation:

```css
.dashedborder {
    border: 3px dashed #000033;
    /* border-width border-style border-color */
}
```
---

### Padding Properties