# Positioning

`position: static relative absolute fixed;`

position element = value other than static

`position element = top, left, bottom, right;`

- `relative` = only shifts when using positioning properties
- `absolute` = manual positioning
- `fixed` = gives it a specific place, no matter what

###Static Positioning

- rendering in normal flow

### Fixed Positioning

- stays in place, even when scrolling down 

### Relative Positioning

- To slightly change location of element
- `top, left, bottom, right;`

**Example:**

```css 
p {
    position: relative; 
    left: 30px;
}
```
### Absolute Positioning

- specifying location of element outside of normal flow
- `top, left, bottom, right;`

**Example:**

```css 
p {
    position: absolute; 
    left: 200px;
    top: 100px;
}
```