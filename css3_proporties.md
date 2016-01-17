
# CSS Properties
- `font: style weight size/line-height family ;`
- `background: color(image) repeat x-position y-position;`
- `list-style: style position image;`
- `margin/padding: top right bottom left / top right&left bottom / top&bottom right&left;`
- `border: width style color;`
- `display: none / block / inline / inline-block;`



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


  