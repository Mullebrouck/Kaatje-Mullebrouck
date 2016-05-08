# String Manipulation

### .toUpperCase(); 

```js
var sentence = "Example of a string."
var upperCase = sentence.toUpperCase();  // EXAMPLE OF A STRING.
```

### .toLowerCase(); 

```js
var sentence = "ExaMPle of a StriNg."
var lowerCase = sentence.toLowerCase(); // example of a string.
```

### .split(); 

```js
var sentence = "Example of a string."
var words = sentence.split(" "); // ["Example", "of", "a", "string."]
```
--> Needs a space (" ") in order for it to work. Because it shows you where the string should split up, in this case after the space. (This could be a comma, ...)

### .slice(); 

```js
var sentence = "Example of a string."
var word = sentence.slice(3, 8); // mple 
```

### .indexOf(); 

```js
var sentence = "Example of a string."
var position = sentence.indexOf("string"); // 13 
```

### charAt() ; 

Returning letter in string

```js
var sentence = "Example of a string."
var position = sentence.charAt(4); // p
```
