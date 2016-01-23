# Image Maps

= image that is used as one or more hyperlinks. 

- **Selectable area**  = hotspot

- **Selected areas can come in 3 shapes:**
    - rectangle
    - circle
    - polygon
    

- **requires**: 

    - image element
    - map element
    - one or more elements
    
    
###Map Element

= indicated beginning and ending of image description

```html
<map name="image name" id="Same as image name"> 
    
</map>
```

###Area Element

= coordinates or edges of clickable area

**Used Tags:**

- href = website tag refers to
- alt = text for screen readers
- title = text for tooltips
- shape = shape
- coords = coordinate position of clickable area

Shape Coordinates: 

| Shape | Coordinates | 
| -- | -- | -- |
| rect | "x1,y1, x2,y2" |
| circle |"x,y,r" |
| polygon | "x1,y1 x2,y2, x3,y3, ..."|


Example: 

```html
<map name="house" id="house">
    <area 
        href="http://www.house.com" 
        shape="rect"
        coords="24, 188, 339, 283"
        alt="house"
    >
</map>
<img 
    src="house.jpg"
    usemap="#house"
    alt="house and garden"
    width="416"
    hight="350"
>

```

Free Online Map Generators: 

- http://image-maps.com
- http://mobilefish.com/services/image_map/image_map.php




