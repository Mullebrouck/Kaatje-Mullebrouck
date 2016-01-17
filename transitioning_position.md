# Transitioning Position


##Transitioning in Hidden Button Content

Original Button

```html
<section>
    <a href="#" class="btn button">
    Text for Button
    </a>
</section>
    
```

### 1. Create 2 inner spans

Holds current and additional information shown on button hover:

```html
<section>
    <a href="#" class="btn button">
        <span class="top-content">Top Content of btn </span>
        <span class="bottom-content>Bottom Content btn </span>
    </a>
</section>
    
```

### 2. Style initial and hover state

Initial state:

```css
.btn {position: relative;}
.content {position: absolute;}

.top {top:0;}
.bottom {top: 100px;}
```
>Always put in .bottom 100px, so you can't see it.

Hover State:

```css
.btn {position: relative;}
.content {position: absolute;}

.top {top:0;}
.btn:hover .top {top: -100px;}
.bottom {top: 100px;}
.bottom:hover .bottom {top:0px;}
```


