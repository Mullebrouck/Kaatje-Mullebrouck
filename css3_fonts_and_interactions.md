# CSS3 Fonts and Interactions

### Importing web font face

```css
@font-face {
 font-family: 'OpenSansRegular';
 src: url('OpenSansRegular-webfont.eot'); 
   (don't forget to add more font types by adding additional url()'s)
 font-style: normal;
 font-weight: normal;
}

h1 {
 font-family: 'OpenSansRegular', Helvetica;
}
```
You can use different weights with @font-face
```css
@font-face {
 font-family: 'OpenSansRegular';
 src: url('OpenSansBold-webfont.eot'); 
 font-style: normal;
 font-weight: bold;
}

h1 {
 font-weight: bold, Helvetica;
}
```

### Transforms

To translate, rotate, skew and scale elements in CSS

**translate**

Creating 2D translation
```css
.element {
  transform: translate (<transition-value X-axis>, <transition-value y-axis>);
}
```
Translate Individually:
```css
.element {
 transform: translateX(VALUE);
}
.element {
 transform: translateY(VALUE);
}
```
length or percentage, if not specified = 0

**rotate**

.element {
 transform: rotate(VALUE deg);
}
```

**scale**
```css
.element {
 transform: scale(<x-axis>, <y-axis> );
}
```
if not specified default is `<x-axis>`

Translate Individually:
```css
.element {
 transform: scaleX(VALUE);
}
.element {
 transform: scaleY(VALUE);
}
```

**skew**

```css
.element {
 transform: skewX(Angle X-axis);
}
.element {
 transform: skewY(Angle Y-axis);
}
```

### Transitions

```css
 transition: <property> <duration> <timing-function> <delay>;
```
Transition Individually:
```css
.element {
 transition-property: ;
 transition-duration: ;
 transition-timing-function: ;
 transition-delay: ;
}
```
- `<property>` = property you want to transition, if all properties use = all
- `<duration>` = duration transition (default = 0)
- `<time-function>` = timing of transition
(_ease, ease-in, ease-in-put, linear, cubic-bezier, step-start, step-end, steps()_)
- `<delay>` = time of wait between request and start