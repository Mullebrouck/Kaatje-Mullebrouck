# Opacity Property

0 = Completely transparent<br>
1 = completely opaque

>When using opacity property it will effect both your text and background.

___

#RGBA Color

**RGBA = Red, Green, Blue and Alpha (Transparency)**<br>
 --> does not use hexadecimal colors values. 

>Using RGBA will allow you to do only your background or your text


Example:

```css
color: rgba(255, 255, 255, 0.7);
```

= RGB Color is based on hardware
___

#HSLA Color

**HSLA = Hue, Saturation,Lightness and Alpha (Transparency)**<br>

- **Hue**: actual color,  number value: 0-360
- **Saturation**: intensity color
    -  full saturation = 100%
    -  gray = 0%
- **Lightness**: brightness or darkness
    - normal color = 50%
    - white = 0%
    - black = 100%
- **Alpha**: Transparency 0-1


###Color Examples: 

- **Red**: hsla(360, 100%, 50%, 1.0);
- **Green**: hsla(120, 100%, 50%, 1.0);
- **Blue**: hsla(240, 100%, 50%, 1.0);
- **Black**: hsla(0, 0%, 0%, 1.0);
- **Gray**: hsla(0, 0%, 50%, 1.0);
- **White**: hsla(0, 0%, 100%, 1.0);


- **Dark Cyan Blue**: hsla(210, 100%, 25%, 1.0);
- **Cyan Blue**: hsla(210, 100%, 50%, 1.0);
- **Light Cyan Blue**: hsla(210, 100%, 75%, 1.0);


= HSLA Color is based on color wheel

