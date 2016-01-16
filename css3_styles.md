# CSS3 Styles

**Border Radius**

Add's Rounded corners to corners

```css
border-radius: ...px; (all borders are the same)
border-radius: <top left> <top right> <bottom right> <bottom left> ;
```
```css
border-top-left-radius:  ;
border-top-right-radius:  ;
border-bottom-right-radius:  ;
border-bottom-left-radius:  ;
```
_To make it a circle use: `50%`_

**Box Shadow**

```css
.box {
  box-shadow: <inset> <offset -x> <offset-y> <blur-radius> <spread-radius> <color> ;
}
```
- `<inset>` = when not specified, you will get a drop shadow
- `<offset -x>` = shadow left and right
- `<offset -y>` = shadow up and down
- `<blur-radius>` = blur amount , gets bigger and lighter with larger value
- `<spread-radius>` = shadow expands or shrinks

Multiple box-shadows:

```css
.box {
  box-shadow:
    ..px ..px ..px #000, 
    inset ..px ..px ..px blue;
}
```
box-shadow <inset> <offset -x> <offset-y> <blur-radius> <spread-radius> <color> ;


**Text Shadow**

```css
.text {
  text-shadow: <offset -x> <offset-y> <blur-radius> <color> ;
}
```

**Box Sizing**

Margins, borders, padding and content.

Three different values for Box-Sizing:

- `box-sizing: content-box;` just content width and Height (Default Value)
- `box-sizing: padding-box;` Width and Height of Content and Padding
- `box-sizing: border-box;` Width and Height of Content, Padding and Border

**Multiple Backgrounds**

Specify background-images in comma-delimited list:
```css
.background {
  background-image: url(Image.png), url(Image2.png);
  background-postition: top left, center right;
  background-repeat: no-repeat, no-repeat;
}
```
or short:
```css 
.background {
  background:
    url(Image.png) top left no-repeat,
    url(Image2.png) center right no-repeat;
}
```

**Color**

RGBa --> a = alpha (opacity)

```css
.color {
  color: rgba(0, 0, 0, 0.75)
}
```

HSLa --> Hue, Saturation, Lightness, Alpha (opacity)

```css
.color {
  color: hsla(Hue, saturation%, ligh%, opacity)
}
```

**Opacity**

```css
.color {
 opacity: ..% ;
}
```
Note: _Opacity will apply to nested elements_


**Gradients**

- Linear Gradients

```css
.gradient {
  background: linear-gradient(<angle> to <side-or-corner>, <color-stop>s);
}
```
-`angle` = in degrees (deg) or use keyword
   + to top --> 0deg
   + to bottom --> 180deg
   + to right --> 270deg
   + to left --> 90deg

-`side-or-corner` = two keywords: Horizontal (left or right) and Vertical (top or bottom)
-`color-stop` = color and stop position (can be length or percentage)


- Radial Gradients

```css
.gradient {
  background: 
    radial-gradient(<shape> <size> at <position>, <color-stop>s);
}
```
- `shape` = circle or ellipse(default)
- `size` = closest-side, closest-corner, farthest-side, farthest-corner(default) --> length or percentage
- `position` = same as background-position (center = default)
- `color-stop` = color and optional stop position --> length or percentage