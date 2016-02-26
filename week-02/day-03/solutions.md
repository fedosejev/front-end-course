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