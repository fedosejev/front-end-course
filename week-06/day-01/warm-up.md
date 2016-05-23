# Warm up

## 0.

```js
var whiteTesla = {
  name: 'Model X'  
};

var redTesla = whiteTesla;

redTesla.name = 'Model S';

console.log(whiteTesla.name); // ???
```

What will be logged and why?

+ [Example](https://repl.it/ByF1/0)

## 0.1

```js
var models = ['Model S', 'Model X'];
var teslas = models;
teslas[2] = 'Model 3';

console.log(models[2]); // ???
```

What will be logged and why?


+ [Example](https://repl.it/ByFc/0)

## 0.2

```js
var list = [];

function addOne(items) {
    items.push(1);
}

function addTwo(items) {
    items.push(2);
}

function addThree(items) {
    items.push(3);
}

addOne(list);
addTwo(list);
addThree(list);

console.log(list); // ???
```

What will be logged and why?

## 1.

Write a function `getValue` that takes 2 parameters: 1) object and 2) key name and returns a value for that key in that object.

How to test:

```js
var model = {
  name: 'Model S'
};

var value = getValue(model, 'name');

console.log(value); // 'Model S'
```

+ Use [Repl.it](https://repl.it) instead of jsBin.

## 2.

Write a function `logFirst` that takes 2 parameters: 1) an array of numbers and 2) a function that logs a number, then `logFirst` logs the first number in the array.

How to test:

```js
logFirst([100, 500, 900], console.log); // 100
```

+ Use [Repl.it](https://repl.it) instead of jsBin.

## 3.

Write a function `logAny` that takes 3 parameters: 1) an array of numbers and 2) a number that represents the nth item in that array and 2) a function that logs a number, then `logAny` logs the nth number in the array.

How to test:

```js
logAny([100, 500, 900], 3, console.log); // 900
```

+ Use [Repl.it](https://repl.it) instead of jsBin.

## 4.

![](https://45.media.tumblr.com/04a67b7ef443fe6f1300a3b113f8037a/tumblr_noxmlwv1841qbls2ko1_500.gif)

Solve problems `1`, `1.1`, `1.2` and `1.3`: https://github.com/fedosejev/javascript-problems#1
