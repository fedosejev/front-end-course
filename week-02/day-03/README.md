# Day 3

![](https://33.media.tumblr.com/tumblr_lmfix57faG1qhq4cpo1_400.gif)

Questions:

+ [What is value?](#what-is-value)
+ [What is variable?](#what-is-variable)
+ [What is statement?](#what-is-statement)
+ [What is expression?](#what-is-expression)
+ [What is expression statement?](#what-is-expression-statement)
+ [What is operator?](#what-is-operator)
+ [What types JavaScript defines?](#what-types-javascript-defines)
+ [What subtypes JavaScript defines?](#what-subtypes-javascript-defines)
+ [How do I declare a variable?](#how-do-i-declare-a-variable)
+ [How do I assign value to a variable?](#how-do-i-assign-value-to-a-variable)
+ [What is Statement Completion Value?](#what-is-statement-completion-value)
+ [What is `for` loop?](#what-is-for-loop)
+ [How to break from `for` loop?](#how-to-break-from-for-loop)
+ [What is `while` loop](#what-is-while-loop)
+ [How to break from `while` loop?](#how-to-break-from-while-loop)
+ [What is `do while` loop?](#what-is-do-while-loop)

Plus:

+ [Problems](#problems)

## Questions

### What is value?

Value has a type.

```js
42; // The type is number
```

```js
'Hello'; // The type is string
```

```js
[]; // The type is array
```

```js
{}; // The type is object
```

### What is variable?

Variable has no type.

```js
var message;
```

### What is statement?

> In a computer language, a group of words, numbers, and operators that performs a specific task is a _statement_.

```js
a = b * 2;
```

> The characters a and b are called variables.

> In programs, variables hold values (like the number 42) to be used by the program.

> By contrast, the 2 is just a value itself, called a literal value, because it stands alone without being stored in a variable.

> The `=` and `*` characters are operators - they perform actions with the values and variables such as assignment and mathematic multiplication.

> Most statements in JavaScript conclude with a semicolon (;) at the end.

> The statement a = b * 2; tells the computer, roughly, to get the current value stored in the variable b, multiply that value by 2, then store the result back into another variable we call a.

### What is expression?

> Statements are made up of one or more _expressions_.

> Expressions evaluate to values.

Example:
```js
a = b * 2;
```

> This statement has four expressions in it:
+ `2` is a _literal value expression_
+ `b` is a variable expression, which means to retrieve its current value
+ `b * 2` is an arithmetic expression, which means to do the multiplication
+ `a = b * 2` is an assignment expression, which means to assign the result of the b * 2 expression to the variable `a`.

### What is expression statement?

+ `b * 2;`
+ `log(a);` - _call expression_ statement

### What is operator?

#### Assignment operators

Assign a value to a variable.

```js
color = 'Yellow';
```

#### Arithmetic operators

Perform basic math.

```js
days = 12 * 5;
```

+ Addition: `+`
+ Subtraction: `-`
+ Division: `/`
+ Multiplication: `*`
+ Increment: `++`
+ Decrement: `--`
+ Modulus: `%`

#### String operators

Combine (concatenate) two strings.

```js
message = 'Welcome to' + ' ' + 'The Iron Yard';
```

#### Comparison operators

Compare two values and return `true` or `false`.

```js
3 > 5;
```

#### Logical operators

Combine expressions and return `true` and `false`.

```js
(a === b) && (1 < 10);
```

### What types JavaScript defines?

JavaScript defines seven built-in types:

+ `null`
+ `undefined`
+ `boolean`
+ `number`
+ `string`
+ `object`
+ `symbol` - added in ES6.

All of these types except object are called "primitives".

The `typeof` operator inspects the type of the given value.

### What subtypes JavaScript defines?

+ `function` is a subtype of `object` and it's a "callable object".
+ `array` is a subtype of `object`.

> In JavaScript, __variables don't have types - values have types__. Variables can hold any value, at any time.

### How do I declare a variable?

```js
var a;
```

### How do I assign value to a variable?

```js
a = 100;
```

### What is Statement Completion Value?

> Statements all have completion values.

Execute the following statement in Chrome's JavaScript console:

```js
var a = 100;
```

`undefined` will be printed out - this is a statement completion value.

### What is `if` statement?

```js
if (condition) {
  // true
}
```

```js
if (condition) {
  // true
} else {
  // false
}
```

```js
if (condition) {
  // true
} else if (condition) {
  // true
}
```

```js
if (condition) {
  // true
} else if (condition) {
  // true
} else {
  // both are false
}
```

+ Learn more: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else

### What is `for` loop?

Use `for` loop when you need to run code a specific number of times.

```js
for (initialization; condition; update) {
  // code block
}
```

+ `initialization` - do something before the first loop.
  + Example: variable declaration and initialization: `var iterator = 0`
+ `condition` - `true` or `false` - decide whether to break from for loop or run the code block.
  + Example: `iterator < 10`
+ `update` - update after every loop.
  + Example: `iterator++`

Example:

```js
for (var iterator = 0; iterator < 10; iterator++) {
  console.log(iterator);
}
```

Logs:

```js
0
1
2
3
4
5
6
7
8
9
```

+ [Example](http://jsbin.com/banivi/edit?js,console)

### How to break from `for` loop?

Use `break` statement:

```js
for (var iterator = 0; iterator < 10; iterator++) {
  if (iterator === 5) {
    break;
  }

  console.log(iterator);
}
```

Logs:

```js
0
1
2
3
4
```

+ [Example](http://jsbin.com/hapufa/edit?js,console)

### What is `while` loop?

Use `while` loop if you don't know how many times the code should run.

```js
while (condition) {
  // code block
}
```

Example:

```js
var iterator = 0;

while (iterator < 10) {
  console.log(iterator);
  iterator++;
}
```

Logs:

```js
0
1
2
3
4
5
6
7
8
9
```

+ [Example](http://jsbin.com/hereve/edit?js,console)

### How to break from `while` loop?

```js
var iterator = 0;

while (iterator < 10) {
  if (iterator === 5) {
    break;
  }
  console.log(iterator);
  iterator++;
}
```

+ [Example](http://jsbin.com/qaxinu/edit?js,console)

### What is `do while` loop?

Use `do while` loop if you need to execute code block at least once.

```js
do {
  // code block
} while (condition);
```

Example:

```js
var iterator = 0;

do {
  console.log(iterator);
  iterator++;
} while (iterator === -1);
```

Logs:

```js
0
```

+ [Example](http://jsbin.com/niyohe/edit?js,console)

You can break from `do while` loop in the same way as with `while` loop.

## [Problems](problems.md)

## Learn more

1. [You Don't Know JS: Up & Going: Chapter 1: Into Programming](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch1.md)
2. [You Don't Know JS: Scope & Closures: Chapter 1: What is Scope?](https://github.com/getify/You-Dont-Know-JS/blob/master/scope%20%26%20closures/ch1.md)
2. [Mastering The Developer Tools Console](http://blog.teamtreehouse.com/mastering-developer-tools-console)
