# Arrays


## Working with arrays

example: 

```js
var list = [1, 2, 3, 4, 5, 6, 7, 8, 9];
```
<br>


### adjusting numbers in array



example: 

```js
var list = [1, 10, 3, 4, 5, 6, 7, 8, 9]; 
```
Now we want to change the number 10 into number 2:

```js
list[1] = "2"

//this will make the outcome like this: 

var list = [1, 2, 3, 4, 5, 6, 7, 8, 9];
```

### Deleting last position in array

```js
list.pop();

//this will delete the last position: 

var list = [1, 2, 3, 4, 5, 6, 7, 8];
```
you can store the last data into a variable 

```js
var newList = list.pop();
```

### Adding a position in array

```js
list.push("10");

//this will add anorher position: 

var list = [1, 2, 3, 4, 5, 6, 7, 8, 10];
```
