# Warm up

# 1.

Write a function that takes a parameter as an object where each value is an array of numbers and returns an object where each value is a sum of these numbers.

Example:

```js
var results = sumAll({
  'AAPL': [20, 50, 70],
  'TSLA': [100, 90, 30, 75],
  'AMZN': [10, 60]
});

console.log(results); // { 'AAPL': 140, 'TSLA': 295, 'AMZN': 70 }
```