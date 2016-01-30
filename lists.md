# Lists

##Unordered list/ordered list

- will show a disc mark
- use `list-style-property` to configure style of list marker

### list-style-type Property

- `none` = no display 
- `disc` = circle 
- `circle` = open circle
- `square` = square
- `decimal` = decimal numbers
- `upper-alpha` = uppercase letters
- `lower-alpha` = lowercase letters
- `lower-roman` = lowercase roman numerals

### list-style-image Property

- will replace bullet points into image
- as value you use: The url keyword with parenthesis surrounding filename or path for the image. 

Example: 
```css
ul { 
    list-style-image: url(filename);
}
```

### list-style-position Property

- placement of list markers
- `inside` = markers are indented
- `outside` = default, default placement