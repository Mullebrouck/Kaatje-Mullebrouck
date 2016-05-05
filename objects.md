# Objects

= container for information

Declaring and defining (No classes in JavaScript, only objects)



## Notation:

**Literal Notation**

```js 
var myObject = {
  key: value, 
  key: value, 
  key: value
};
```
or shorter notation: 

```js
var myObject = {key: value, key: value, key: value, ...};
```

**Constructor Notation**

```js 
// Tells you we are creating a new object
var myObj = new Object();

myObj.property = some value;
//or
myObj["property"] = some value;
```
--> Tells you we are creating a new object


## How to add object in array

```js
var newArray = [
    [1, 3], 
    [info = { name: "kaatje", age: 30}]
    ];
```

## Example of Objects with THIS.

```js
//creating 2 objects
var player1 = {name: "Tommy", age: 16, sport: "Baseball"};
var player2 = {name: "James", age: 15, sport: "Soccer"};

function playerDetails(){
  //Display information about each player! Use this.
  console.log(this.name + "favorite sport is " + this.sport + "and is " + this.age + " years old."); 
}

player1.logDetails = playerDetails; 
player2.logDetails = playerDetails; 

player1.logDetails();
player2.logDetails();

```
