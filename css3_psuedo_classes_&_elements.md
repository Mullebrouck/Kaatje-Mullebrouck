# CSS3 Psuedo Classes & Elements

#Psuedo Classes

start with `:` = selecting element based on state and position

```css
:first-child / :last-child / :only-child
```
**links**
```css
:hover / :focus / :active / :visited
```
**nth-child**
```css
:nth-child() / :nth-of-type()
```
`:nth-child(an + b)` = intervals of a, starting with element at position b or 0

- `:nth-child(even)` = selecting even elements
- `:nth-child(odd)` = selecting odd elements
- `:nth-child(2n)` = selecting even elements
- `:nth-child(2n+1)` = selecting odd elements
- `:nth-child(3n+3)` = selecting every third element
- `:nth-child(4n+4)` = selecting every fourth element
- `:nth-child(3n+1)` = selecting every third element starting at number 1

#Psuedo Element

- ` :before / :after `
- ` :first-letter / :first-line`

To use always add `content:' ' ` element:

```css
figure:before; {
  content: ' ';
  background: url(IMAGE);
  ....
}
```


example adding decorative element to last paragraph:

- don't add in `<p>`, but use css instead
```html
<article>
  <p> TEXT TEXT TEXT </p>
  <p> TEXT TEXT TEXT </p>
</article>
```
```css
article p:last-child:after {
  content: CODE FOR DECORATIVE ELEMENT;
}
```

