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



