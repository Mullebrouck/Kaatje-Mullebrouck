
#Opacity Property

= **transparency of an element**

- 0 = completely transparent
- 1 = completely opaque


>Applies to both text and background

Example: 

```css
h1 {
    background-color: #FFFFFF;
    opacity: .6;
    font-size: 4em;
    padding: 10px;
}
```

---
#RGBA Color

= Red, Green, Blue and Alpha (Transparency)

--> Based on hardware 

>Applies to or text or background

Example: 

```css
h1 {
    background-color: #FFFFFF;
    Color: rgba(255, 255, 255, .7);
    font-size: 4em;
    padding: 10px;
}
```
___

#HSLA Color
= Hue, Saturation, Lightness and Alpha

- **Hue**: actual color
    - value: 0-360
- **Saturation**: intensity of color (percent)
    - full color saturation = 100%)
    - gray = 0%
- **Lightness**: brightness or darkness of color (percent)
    - Normal Color = 50%
    - white = 100%
    - black = 0%

###Color Examples: 

- **Red**: hsla(360, 100%, 50%, 1.0);
- **Green**: hsla(120, 100%, 50%, 1.0);
- **Blue**: hsla(240, 100%, 50%, 1.0);
- **White**: hsla(0, 0%, 100%, 1.0);
- **Gray**: hsla(0, 0%, 50%, 1.0);
- **Black**: hsla(0, 0%, 0%, 1.0);


- **Dark Cyan Blue**: hsla(210, 100%, 25%, 1.0);
- **Cyan Blue**: hsla(210, 100%, 50%, 1.0);
- **Light Cyan Blue**: hsla(210, 100%, 75%, 1.0);