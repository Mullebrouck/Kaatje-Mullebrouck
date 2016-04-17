# JavaScript


### if statement

**Notation**

```js
if (condition) {
  doSomething();
} else {
  doSomethingElse();
  }
```

###While loop

```js
while(condition){
  doSomething();
}
```

###For loop

```js 
for(initialization, condition, mutator) {
  doSomething();
}

example: 

for (var i=0; i<9; i++) {
  console.log(i);
}

Result:
0
1
2
3
4
5
6
7
8
```

###For-in loop

```js 
for(item in object or array) {
  doSomething();
}

example: 

var countries = ["Belgium", "Germany", "Mexico", "Spain"]
for(country in countries) {
  console.log(countries[country]);
}

result: 

Belgium
Germany
Mexico
Spain
```