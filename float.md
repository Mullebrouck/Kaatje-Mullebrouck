
# Float

- `float:` = right, left or none
- Specify `width` for floating element, unless it is already specified like an `<img>` 
- key element for multicolumn page layout


---

### Clearing float

- if floated item is taller than non-floated content
- if all content is floating

`clear:` = right, left or both

**Clear float with a Line Break**

- common technique to clear flowt within container element:
 ```css
 .clearleft {
    clear:left;
    }
 ```
 ```html
 <div>
    <img class="float" src="yls.jpg" alt="Yellow Lady Slipper" height="100" width="100">
    <p> The Yellow Lady Slipper grows in wooded areas and blooms in June each year. The flower is a member of the orchid family. </p>
    <br class="clearleft">
 </div>
 ```

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