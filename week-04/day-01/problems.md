# Problems

## 1.

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

## 2.

Modify project from the Week 3:

1. Instead of images changing every 3 seconds, make sure user can navigate images by clicking on the thumbnails.
2. Add left arrow button that shows the previous image.
3. Add right arrow button that shows the next image.

## 3.

Write a function `getTotalPrice()` that logs the total price.

Given this object:

```js
var shoppingBasket = {
  products: [
    {
      name: 'iPhone 6S 64GB',
      price: 619
    },
    {
      name: 'iPad Air 2 64GB',
      price: 479
    },
    {
      name: 'Apple Watch',
      price: 519
    }
  ]
};
```

This is how you should call `getTotalPrice()` function:

```js
var totalPrice = getTotalPrice.call(shoppingBasket);

console.log(totalPrice); // "£1617"
```

It should log £1617.