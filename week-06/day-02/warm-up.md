# :fire: Warm :fire: up :fire:

## 1.

What will be logged and __why__?

```js
console.log(console.log(console.log('console.log')));
```

## 2.

Explain:
+ Why do we need lexical scopes?
+ Why do we need closures?
+ Why do we need `this`?
+ Why do we need behaviour delegation?

## 3.

Write the following function:

```js
console.log('hello'.repeatify(3)); // hellohellohello
``` 

## 4.

What will be logged and __why__?

```js
(function () {
  var message = info = 'Introduction';
})();

console.log(typeof message !== 'undefined'); // ???
console.log(typeof info !== 'undefined'); // ???
```

What about now?

```js
(function () {
  'use strict';
  var message = info = 'Introduction';
})();

console.log(typeof message !== 'undefined'); // ???
console.log(typeof info !== 'undefined'); // ???
```

## 5.

What is IIFE good for?

```js
(function () {})();
```

## 6.

What will be logged and __why__?

```js
var car = {
  make: 'Tesla',
  model: 'Model X',
  whatAreYou: function () {
    var that = this;
    console.log(that.make); // ???
    console.log(this.make); // ???
    (function () {
      console.log(that.model); // ???
      console.log(this.model); // ???
    })();
  }
};

car.whatAreYou();
```

## 7.

What will be logged and __why__?

```js
function getData(data, callback) {
  setTimeout(function () {
    callback(data);
  }, 1000);
}

getData(10, function (firstNumber) {
  var x = 1 + firstNumber;

  getData(30, function (secondNumber) {
    var y = 1 + secondNumber;

    getData('Meaning of life: ' + (x + y), function (answer) {
      console.log(answer);
    });
  });
});
```

## 8.

Write function `sum` that returns the same answer in both cases:

```js
console.log(sum(5, 10)); // 15
console.log(sum(5)(10)); // 15
```