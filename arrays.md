# Arrays


## Working with arrays

example: 

```js
var list = [1, 2, 3, 4, 5, 6, 7, 8, 9];
```
<br>

### getting value in array

example: 

```js
var list = [1, 10, 3, 4, 5, 6, 7, 8, 9]; 
list[3];
```
--> 4

### assigning numbers in array


example: 

```js
var[5] = "test";
var list = [1, 10, 3, 4, 5, "test" , 7, 8, 9]; 
```

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
console.log(newList);
```
 --> 9
### Deleting first position in array

```js
list.shift();

//this will delete the first position: 

var list = [2, 3, 4, 5, 6, 7, 8, 9];
```
you can store the first data into a variable

```js
var newList = list.shift();
console.log(newList);
```
 --> 1

### Adding a position in array

```js
list.push("10");

//this will add anorher position: 

var list = [1, 2, 3, 4, 5, 6, 7, 8, 10];
```

###Calling positions in several arrays

```js
var list = [1, 2, 3, 4, 5];
var newlist = [6, 7, 8, 9];
var listingPosition = [list, newlist];
```
We want to create a new variable "position" that is storing number 9

```js
var position = listingPosition[1][3];
```

###getting length in array

```js
var list = [1, 2, 3, 4, 5, 6, 7, 8, 9];
list.length();
```
--> 9

###joining the array with .join( );

```js
var name = ["John", "Doe"];
var full = name.join();
console.log(full);
```
-->John,Doe
```js
var name = ["John", "Doe"];
var full  =  name.join(" ");
console.log(full);
```
-->John Doe

```js
var name = ["John", "Doe"];
var full  =  name.join("and");
console.log(full);
```
-->John and Doe


###returning full array with .map( );

list.map();

```js
var list = [1, 2, 3, 4, 5, 6, 7, 8, 9]; 
list.map(function(num){
  return num * 10; 
});
console.log(result); 
```
--> [10, 20, 30, 40, 50, 60, 70, 80, 90]

