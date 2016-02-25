# Problems

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
