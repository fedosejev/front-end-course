# Warm up

## 1.

Write a function `Tesla` that can used like this:

```js
var modelS = new Tesla('Model S');

modelS.start(); // 'Started Model S'
modelS.stop(); // 'Stopped Model S'
```

## 2.

Given a button:

```html
<button data-price="100.88">Get price</button>
```

Write a function that renders a price underneath the button when user clicks on that button.

You don't need to create this button with JavaScript.

## 3.

Write a function that takes two parameters: 1) an array of objects where each object has `message` property, 2) function that logs a comment message. This function then logs all comments.

```js
var getMessage = function () {
  console.log('Comment:', this.message);
};

var comments = [
  {
    message: 'Yesterday'
  },
  {
    message: 'Today'
  },
  {
    message: 'Tomorrow'
  }
];
```

## 4.

Produce a simplest example of a closure.

## 5.

Given 3 function in a global scope create a new function in a global scope that will encapsulate those 3 functions in a private scope. You should still be able to call `restart` from the global scope.

```js
function on() {
  console.log('On');
}

function off() {
  console.log('Off');
}

function restart() {
  off();
  on();
}
```