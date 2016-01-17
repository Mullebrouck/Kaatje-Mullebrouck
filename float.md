
# Float

`float:` = right, left or none


---



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