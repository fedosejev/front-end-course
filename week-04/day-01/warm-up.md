# Find and fix errors

![](https://metrouk2.files.wordpress.com/2014/03/ghostbusters.gif)

## 1.

```js
function createMessage() {
  var message = 'Welcome to the Iron Yard!';

  function getMessage() {
    return message;
  }
}

var message = getMessage();
```

1 error.

## 2.

```js
var list = window.querySelectorAll('ul');
li.setAttribute('class', 'new');
```

2 errors.

## 3.

Find out how many `div` elements the home page of your web browser has.

## 4.

```js
var element = document.getElementById('city')
element.textContent('London')
```

3 errors.

## 5.

```js
var message;

message + '<p>Address: ' + document.URL + '</p>';

var footerElement = document.getElementById('footer');
footerElement.innerHTML = message;
```

1 error.

## 6.

```js
var car = {
  start: function () {
    return 'Started...';
  }
  stop: function () {
    return start;
  }
};
```

2 errors.

## 7.

Write a function `flip` that takes object as a parameter and returns a new object with keys that are values from original object and values that are keys.

For example:

```js
var result = flip({
  a: 1,
  b: 2,
  c: 3
});

console.log(result); // { 1: 'a', 2: 'b', 3: 'c' }
```
