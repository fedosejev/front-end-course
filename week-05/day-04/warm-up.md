# Warm up

## 1.

Write a function `mix` that takes `firstObject` object as a parameter. Then you call `mix` on `secondObject` object and it returns a new object that has keys from `firstObject` and `secondObject`.

For example:

```js
var firstObject = {
  name: 'Art',
  city: 'London'
};

var secondObject = {
  country: 'United Kindgom',
  position: 'Instructor'
};

var result = firstObject.mix(secondObject);

console.log(result);

/*

{
  name: 'Art',
  position: 'Instructor',
  city: 'London',
  country: 'United Kingdom'
}

*/
```

