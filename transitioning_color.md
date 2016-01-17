# Transitioning Color


Duration = period of time

| CTA = Call to Action (ex. “buy now” button) |
| -- |

---

### Transition Recipe

```css
.btn{
    transition: <property> <duration> <timing-function> <delay>;
}
```
 > Only one that needs to specified is “duration”, all the rest has defaults 
 
```< property >``` = defaults to all

```< timing-function >``` = default to ease

```< delay >``` = defaults to 0
 
 
 Full list of properties that can be transitioned: 
 https://www.w3.org/TR/css3-transitions/#properties-from-css

---

###Transitioning Background Color


```html
   < a href="#" class="btn" >
   Text for Button 
   </a>
```

```css
.btn {
    background-color: #00A0D6;
}
.btn:hover {
    background-color: #007DA7;
}
```
[](codepen://Kaatje/pen/RrLYMj?editors=110)

>To make transition we add in .btn
```
transition: <property> <duration>;
```

```css
.btn {
    background-color: #00A0D6;
    transition: background-color 0.4s;
}
.btn:hover {
    background-color: #007DA7;
}
```



---


### Transitioning Multiple Properties

```css
.btn {
    background-color: #00A0D6;
    color: #FFFFFF;
    transition: background-color 0.4s, color 0.4s;
}
.btn:hover {
    background-color: #007DA7;
    color: #e3e3e3;
}
```


---


### Transitioning All Properties

> Use the “all” as property, BUT every property that can animate will animate

```css
.btn {
    background-color: #00A0D6;
    color: #FFFFFF;
    transition: all 0.4s;
}
.btn:hover {
    background-color: #007DA7;
    color: #e3e3e3;
}
```



