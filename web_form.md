# Web Form

### Setting up the form in HTML

```html
<form>
  <label>NAME</label> (describes what user needs to do)
  <input type="text">
  <input type="submit" value="Click to submit">
</form>
```


**different input types: **

```html
<input type="text"> user-typed text
<input type="checkbox"> checkbox
<input type="radio">
<input type="file"> choose file
<input type="password"> password
<input type="submit"> submit button
```


**Multiple lines of text:**

using `<textarea> </textarea>`

```html
<form>
  <label for="UNIQUE NAME 1">NAME</label>
  <textarea id="UNIQUE NAME 1"></textarea>
  <input type="submit" value="Click to submit">
</form>
```

Note: you can change width and height for textarea with `border `and `margin`


**Attributes `for` and `id`**

value in `for` and `id` should be the same to associate label and input (each `for` and `id` has to be unique on the page)

```html
<form>
  <label for="UNIQUE NAME 1">NAME</label>
  <input type="text" id="UNIQUE NAME 1">
  <input type="submit" value="Click to submit">
</form>
```



**Adding a checkbox**

newsletter label and input are better on the same line!

```html
<form>
  <label for="Newsletter">Get Newsletter?</label>
  <input type="checkbox" id="Newsletter">
</form>
```

```css
input[type=checkbox], label[for=newsletter] {
  display: inline;
}
```


### Styling forms in CSS

labels and inputs are inline-level tags, better to display them on top of each other like block-level instead of side-by-side.

```css
label, input {
  display: block;
}
```


**Adding space between labels and input**

```css
label {
  margin-bottom: ...px;
}
input {
  width:...px;
  margin-bottom: ...px;
}
```


**Adjusting submit button with `attribute selector`**

```css
input {
  width:...px;
  margin-bottom: ...px;
}
input[type=submit] {
  width:...px;
  font-size: ...px;
}
```

type = name of the attribute
submit = value of the attribute



**Styling inputs with the `attribute selector`**

style of input text:

```css
input[type=text] {
  border: 1px solid #234532
}
```

Note: _To adjust height of input, you need to change the style of the text inside!_ or _you can change the padding_