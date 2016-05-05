# Date method

```js
var today = new Date(); 
```

**Example: **

```js
var today = new Date(2000,5,19);
```

###.getMonth();

```js
today.getMonth(); // 5
```

###.getFullYear();

```js
today.getFullYear(); // 2000
```

###.getDate();

```js
today.getDate(); // 19
```

###.getDay();

```js
today.getDay(); // 1 (Monday)
```
--> 0 = Sunday

###.getHours();

```js
today.getHours(); 
```
--> 0 - 23

###.getTime();

```js
today.getTime();
```

--> Milisecond since 1/1/1970

### Comparing Dates

```js

var date1 = new Date(2000,5,19); 
var date2 = new Date(2000,5,19); 

if(date1 == date2) {...} //false

if(date1.getTime() == date2.getTime() {...} //true!
```


###Setting a date

```js
var today = new Date(); 

today.setMonth(8); 
today.setFullYear(); 
```
