## 1.

Write a function named 'printOddAndEvenNumbers' that runs a for loop 10 times and for all odd numbers prints: 'Odd number' and for all even numbers prints: 'Even number'.

1. Write a function named 'printOddAndEvenNumbers'.
2. Create a for loop.
3. Runs 10 times.
+ 3.1 Create iterator.
+ 3.2 Create condition.
+ 3.3 Create update.
4. For all odd numbers prints: 'Odd number'.
  4.1 Check if number is odd.
    4.1.1 Create if statement.
    4.1.2 Create condition.
  4.2 Print 'Odd number'.
5. For all even numbers prints: 'Even number'.

```js
function printOddAndEvenNumbers() {
  var iterator = 0;
  
  for (; iterator < 10; iterator = iterator + 1) {
    if (iterator % 2 !== 0) {
      console.log('Odd number');
    } else {
      console.log('Even number');
    }
  }
}
```

## 2.

```js
function getListLength(list) {
  return list.length;
}
```

## 3.

```js
function reverseArray(list) {
  var reversedList = [];

  for (var iterator = list.length - 1; iterator >= 0; iterator = iterator - 1) {
    var lastItemInTheOriginalList = list[iterator];
    var nextEmptyIndexInTheReversedList = reversedList.length;    
    
    reversedList[nextEmptyIndexInTheReversedList] = lastItemInTheOriginalList;
  }
  
  return reversedList;
}
```