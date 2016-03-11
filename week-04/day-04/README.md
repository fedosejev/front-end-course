# Day 4

+ [Hacking Your Career](https://github.com/fedosejev/hacking-your-career)
+ [Search Algorithms](https://github.com/fedosejev/algorithms)

## What is Recursion?

> When you call a function that calls itself.

### Fibonacci number

+ [Fibonacci number](https://en.wikipedia.org/wiki/Fibonacci_number)

```js
function fibonacci(number) {
  if (number === 0) {
    return 0;
  }

  if (numebr === 1) {
    return 1;
  }

  return (fibonacci(number - 1) + fibonacci(number - 2));
}
```

### Infinite recursion

```js
function process() {
  process();
}
```