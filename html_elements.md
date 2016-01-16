# HTML Elements

**Section**

if all content is related to each other, you can put it in a section instead of div:

Instead of: 
```html
<div class="section">
 <h1>TEXT</h1>
</div>
```
Make it: 
```html
<section>
 <h1>TEXT</h1>
</section>
```
Note: _Outline will not change when you use `<h1>` inside of the `<section>`_


**Header**

Instead of: 
```html
<div class="header">
 <...>
</div>
```
Make it: 
```html
<header>
 <...>
</header>
```
Note: _You can have multiple header elements, even in `<section>`_

**Footer**

Instead of: 
```html
<div class="footer">
 <...>
</div>
```
Make it: 
```html
<footer>
 <...>
</footer>
```

**Aside**

Not exactly related to content, but expand the content. 
- within `<article>`, `<aside>` should be related to that article
- outside `<article>`, `<aside>` should be related to the site (ex. sidebar)

```html
<aside>
 <...>
</aside>
```

**Nav**

Section with navigation links --> used for major navigation

```html
<nav>
  <ul>
    <...>
  </ul>
</nav>
```

**Article** 

- blog post
- news story
- comment post
- review 

```html
<article>
  <...>
</article>
```


**Main**

Main content of your document

- Do NOT have more than 1 `<main>` in doc
- Do NOT include `<main>` in other elements

```html
<main>
  <...>
</main>
```


**Figure/Figcaption**

Common use `<figure>`: for image within `<article>`
```html
<figure>
  <img src="image.png" alt="...">
</figure>
```

Figcaption = caption or legend for `<figure>`

```html
<figure>
  <img src="image.png" alt="...">
  <figcaption>CAPTION FOR PICTURE</figcaption>
</figure>
```

**Time**


```html
<time datetime="yyy-mm-dd">mm/dd/yyyy</time>
```

