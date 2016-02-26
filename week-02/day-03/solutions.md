## 1.

Write a function named 'printOddAndEvenNumbers' that runs a for loop 10 times and for all odd numbers prints: 'Odd number' and for all even numbers prints: 'Even number'.

<ul>
  <li>1. Write a function named 'printOddAndEvenNumbers'.</li>
  <li>2. Create a for loop.</li>
  <li>3. Runs 10 times.</li>
  <ul>
    <li>3.1 Create iterator.</li>
    <li>3.2 Create condition.</li>
    <li>3.3 Create update.</li>
  </ul>
  <li>4. For all odd numbers prints: 'Odd number'.</li>
    <li>4.1 Check if number is odd.</li>
      <li>4.1.1 Create if statement.</li>
      <li>4.1.2 Create condition.</li>
    <li>4.2 Print 'Odd number'.</li>
  <li>5. For all even numbers prints: 'Even number'.</li>
</ul>

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