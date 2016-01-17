
# CSS Properties
- `font: style weight size/line-height family ;`
- `background: color(image) repeat x-position y-position;`
- `list-style: style position image;`
- `margin/padding: top right bottom left / top right&left bottom / top&bottom right&left;`
- `border: width style color;`
- `display: none / block / inline / inline-block;`

# Float

`float:` = right, left or none

### Clearing float

- if floated item is taller than non-floated content
- if all content is floating

`clear:` = right, left or both

**Subsequent Element**

- targeting an element after a floating target and use `clear: both;`
```html
<div>
 <img src="test.png" alt="test">
</div>
<div class="element">
 <p> </p>
</div>
```
```css
img {
  float: right;
}
.element {
  clear: both;
}
```
Problems:
- Sequence need to stay intact or it will break if you move things
- background - borders do not extend

**Manual clearing**

- adding empty element 
```html
<div>
  <img src="test.png" alt="test">
  <p> </p>
  < div class ="clear"></div>
</div>
```
```css
.clear {
  clear: both;
}
```
problems:
- requires empty element
- might not be necessary

**The clearfix**

-used on parent, children will be self-cleared
```css
.group: before,
.group: after {
  content: "";
  display: table;
}
.group: after {
  clear: both;
}
.group {
  zoom: 1; 
}
```
```html
<div class="group">
  <img src="test.png" alt="test">
  <p> </p>
</div>
```

# Inheritance & Specifity

**Nested elements automatically inherit parent**

```html
<article class="CLASSNAME">
  <p> example text </p>
</article>
``` 
```css
.CLASSNAME {
  color: #000000;
}
```
**Override parent with nested selectors**
```html
<article class="CLASSNAME">
  <p> example text </p>
</article>
``` 
```css
.CLASSNAME {
  color: #000000;
}
.CLASSNAME p {
  color: #fff;
}
```
**specificity**

Priority of the selector: 

- Important value overwrites all!
`p { color: #555 !important; }` -- always first! (only use when necessary)
- first digit: inline styles  
`<h1 style="color: #543210"> TEXT </h1>` --> 1, 0, 0, 0
- second digit: # of ID selectors
`#header { color: #012345 }` --> 0, 1, 0, 0
- third digit: # of class selectors
`.intro { color: #000000 }` --> 0, 0, 1, 0
- fourth digit: # of element selectors
`p { color: #fff }` --> 0, 0, 0, 1


# Overflow

`overflow: visible auto hidden scroll;`

- `visible` = shows content beyond container boundaries
- `auto` = adds scrollbar when content overflows
- `hidden` = hides overflowing content
- `scroll` = adds scrollbar

- `overflow-x`
- `overflow-y`


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


  