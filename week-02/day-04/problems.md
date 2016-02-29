# Problems

## 0.1.

Write a function `mergeArrays` that takes two arrays as parameters and returns a new array that is made of two arrays merged together.

Example:

```js
mergeArrays([1, 2, 3], [4, 5, 6]); // returns [1, 2, 3, 4, 5, 6]
```

+ [Solution](solutions.md)

## 0.2.

Write a function `updateObjects` that takes an array of objects where each object has a `message` key and a string value.

For each object `updateObjects` must add another key `getMessage` with a value of a function that returns the message in that object.

Example:

```js
var objects = [
  {
    message: 'Please enter your email address.'
  },
  {
    message: 'Please log in.'
  }
];

var updatedObjects = updateObjects(objects);

updatedObjects[0].getMessage(); // 'Please enter your email address.'
```

## 1.

How many lexical scopes you can see here:

```js
function printMessage(message) {
  console.log(message);  
}

function getMessageLength(message) {
  return message.length;
}
```

## 2.

Fix `ReferenceError: askForAddress` error:

```js
deliverProduct();

function deliverProduct() {
  var address = askForAddress();
}

function takeOrder() {
  function askForAddress() {
    var address = {
      houseNumber: '20',
      street: 'Bond Street',
      city: 'London',
      country: 'United Kingdom'
    };

    return address;
  }
}
```

## 3.

Convert this named function into annonymous function:

```js
function sum(a, b) {
  return a + b;
}
```

## 4.

Convert this function into Immediately Invoked Function Expression (IIFE):

```js
function getMessageLength(message) {
  return message.length;
}
```

## 5.

Create a JavaScript object that has a property which you can access like this:

```js
message.explained.translated.comments;
```

## 6.

Write a function that:
1. Takes an array as a parameter
2. Iterates over each value in that array
3. Checks if the value's type is `number`
4. If it is - calculate the sum of all numbers

## 7.

Write an algorithm in JavaScript that sorts and returns an array of 3 numbers, e.g.:

```js
function sortArray(unsortedArray) {
  // ... your code goes here
}
```

To test:
```js
sortArray([2, 12, 7]); // returns: `[2, 7, 12]`
sortArray([1, 34, -27]); // returns: `[-27, 1, 34]`
```

## By the way

![](http://www.explainxkcd.com/wiki/images/e/e6/minifigs.png)
