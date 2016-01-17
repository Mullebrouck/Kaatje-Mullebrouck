
# CSS Properties
- `font: style weight size/line-height family ;`
- `background: color(image) repeat x-position y-position;`
- `list-style: style position image;`
- `margin/padding: top right bottom left / top right&left bottom / top&bottom right&left;`
- `border: width style color;`
- `display: none / block / inline / inline-block;`


# Positioning

`position: static relative absolute fixed;`

position element = value other than static

`position element = top, left, bottom, right;`

- `relative` = only shifts when using positioning properties
- `absolute` = manual positioning
- `fixed` = gives it a specific place, no matter what

# Box Model

- content = `width`
- padding = `padding`
- border = `border`
- margin = `margin`
- Box width = `content width + adding width + border width;`
 

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

### Padding Properties





# Display 

`display: none / block / inline / inline-block;`

###block element
- full width of container
- by default:
`<div> <p> <ul> <ol> <li> <h1 --> h6>`

**centering**
- declare width less than parent
- set `margin: 0 auto;`


###inline element
- found within block - elements
- take up space of content
- no line-break
- by default:
`<span> <a> <em> <img> <strong>`

**centering**
- set `text-align: center;`

###inline-block element
- not by default, needs to be applied
- same flow as inline, but behaves like block

**centering**
- set `text-align: center;`

# Margins

Apply margins to every element to protect layout 
```css
.header {
}
.body {
}
.footer {
}
``` 

###Collapsing margins

Largest margin will be applied, smaller will collapse, unless:
- there is a padding/border
- positioning is relative or absolute
- there is a float left or right


  