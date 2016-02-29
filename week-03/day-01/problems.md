# Problems

## 1.

Make sure variable `message` is defined in a private scope:

```js
var message = 'Welcome!';
```

## 2.

Write `validateParameter` function that takes a parameter, checks whether it's type is string and length is greater than 0.

How to test:
```js
validateParameter(); // returns: false
validateParameter(''); // returns: false
validateParameter(5); // returns: false
validateParameter('Welcome'); // returns: true
```

## 3.

Write `findInList` function that takes 2 parameters: a string and a character and returns a number of times that character is repeated in that string.

How to test:
```js
findInList(); // returns: 0
findInList(''); // returns: 0
findInList('', 'a'); // returns: 0
findInList('Hello', 'a'); // returns: 0
findInList('Again', 'a'); // returns: 2
```

## 4.

Write `squareList` function that takes an array of numbers and returns a new array where each number is squared.

How to test:
```js
squareList(); // returns: []
squareList([]); // returns: []
squareList([2]); // returns: [4]
squareList([2, 4, 1]); // returns: [4, 16, 1]
```

## 5.

Write `filterList` function that takes an array of any values and returns a new array with only non-empty strings.

How to test:
```js
filterList(); // returns: []
filterList([]); // returns: []
filterList(['', 78]); // returns: []
squareList([37, 'Welcome', [], 'back']); // returns: ['Welcome', 'back']
```

## 6.

Write `iterateList` function that takes an array and a function and for each item in that array it calls the function and passes array's item as a parameter.

How to test:
```js
iterateList([1, 2, 3, 4, 5], function (listItem) {
  console.log(listItem);
});
```

## 7.

Write `add` function that adds two numbers, but it needs to be called twice for that.

How to test:
```js
var add5 = add(5);
var sum = add5(10); // returns: 15
```

## 8.

Explain why `undefined` is logged and how to get the actual message logged:

```js
var message = (function () {
  var message = 'Welcome';
  
  function getMessage(message) {
    return message;
  }
  
  return {
    getMessage: getMessage
  };
})();
  
console.log(message.getMessage());
```

## 9. Write `mergeArrays` function:

```js
mergeArrays([1,2,3], ['a', 'b', 'c']); // returns [[1, a], [2, b], [3, c]];
```