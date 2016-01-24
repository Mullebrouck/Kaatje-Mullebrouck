# Box-Shadow Property

= **used to create shadow effect on block-display**

- **Horizontal offset**: px value, 
    - Positive number = shadow on right
    - Negative number = shadow on left
    

- **Vertical offset** : px value, 
    - positive number = shadow on below
    - negative number = shadow above
    

- **Blur radius**: px value, 
    - 0 (default) = sharp shadow
    - higher value = more blur


- ** Spread distance**: px value, 
    - 0 (default)
    - positive number = expanding shadow
    - negative number = contracting shadow


- **Color Value** : shadow in different color

___
Examples: 

- dark gray-drop shadow, 
- 5px horizontal offset, 
- 5px vertical offset, 
- 5px blur radius

```css
box-shadow: 5px 5px 5px #828282;
```

**Inner Shadow Effect**

include optional `inset` value

```css
box-shadow: inset 5px 5px 5px #828282;
```