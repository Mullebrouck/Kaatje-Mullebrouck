# Box Model

- content = `width`
- padding = `padding`
- border = `border`
- margin = `margin`
- Box width = `content width + adding width + border width;`

![](http://www.w3schools.com/css/box-model.gif)
 

---

## Content Properties

- Combination of text and web page elements
- visible width of element = total content width + padding width + border width
- `width` property only configures width of content


## Padding Properties

`padding` property default = 0 

>If you configure background color, color will be applied to padding and content area. 

    padding-bottom
    padding-left
    padding-right
    padding-top


## Border Properties


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

## margin

- determines empty space between element and adjacent elements

### Margin Properties

- configure margins on all sides of the element
- always transparent
- use property to overwrite defaults
- use px or em

> To eliminate: `0`
> 

