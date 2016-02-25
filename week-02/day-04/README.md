# Day 4

Questions:

+ [What is lexical scope?](#what-is-lexical-scope) 
+ [What is function?](#what-is-function)
+ [What is named function?](#what-is-named-function)
+ [What is unnamed or anonymous function?](#what-is-unnamed-or-anonymous-function)
+ [What is function declaration, function expression?](#what-is-function-declaration-function-expression)
+ [What is Immediately-invoked function expression (IIFE)?](#what-is-immediately-invoked-function-expression-iife)
+ [Parameters or arguments?](#parameters-or-arguments)
+ [How to create an array?](#how-to-create-an-array)
+ [How to manipulate arrays?](#how-to-manipulate-arrays)

Plus:

+ [Problems](#problems)
+ [References](#references)

## Questions

### What is lexical scope?

+ [Chapter 1](https://github.com/getify/You-Dont-Know-JS/blob/master/scope%20%26%20closures/ch1.md)

### What is function?

> Function let you group a series of statements together to perform a specific task.

```js
function name(parameter) {
   console.log(parameter);
}

name('Argument!');
```

### What is named function?

```js
function say(message) {
   console.log(message);
}

say('Hello');
```

### What is unnamed or anonymous function?

```js
function () {
   console.log('Hello');
}
```

### What is function declaration, function expression?

#### Function declaration:
```js
function say() {} // Note - no semicolon at the end.
```

+ [Example](http://jsbin.com/xisilop/edit?js,console)

#### Function expression:
```js
var say = function () {};
```

+ [Example](http://jsbin.com/qukuve/edit?js,console)

Explain why you get `TypeError` in that example?

### What is Immediately-invoked function expression (IIFE)?

```js
(function say() {})();
```

+ [Article 1](http://benalman.com/news/2010/11/immediately-invoked-function-expression/)

### Parameters or arguments?

```js
function speak(message) {
  console.log(message);
}

speak('Welcome to The Iron Yard!');
```

+ Parameter: `message`
+ Argument: `'Welcome to The Iron Yard'`

#### Arguments as values

```js
speak('Welcome to The Iron Yard!');
// 'Welcome to The Iron Yard!' is an argument.
```

#### Arguments as variables

```js
var message = 'Welcome to The Iron Yard!';
speak(message);
// message is an argument.
```

### How to create an array?

```js
var array = [1, 2, 3];
```

### How to manipulate arrays?

+ Add item at the end: [`push()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push)
+ Remove the last item: [`pop()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop)
+ Remove the first item: [`shift()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/shift)
+ Add item at the beginning: [`unshift()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/unshift)
+ Remove/add items: [`splice()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)
+ Get a subarray: [`slice()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice)
+ Iterate: [`forEach()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/foreach)

## Problems

+ [7 problems](problems.md)

## Learn more

1. [You Don't Know JS: Scope & Closures: Chapter 1: What is Scope?](https://github.com/getify/You-Dont-Know-JS/blob/master/scope%20%26%20closures/ch1.md)
2. [Immediately-Invoked Function Expression (IIFE)](http://benalman.com/news/2010/11/immediately-invoked-function-expression/)

## Examples

+ http://jsbin.com/hiqube/edit?js,console
+ http://jsbin.com/luyugecazo/edit?js,console
