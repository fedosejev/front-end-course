# Find and fix errors

![](https://metrouk2.files.wordpress.com/2014/03/ghostbusters.gif)

## 1.

```js
var list = [99, 98, 97;

for (iterator < list.length; var iterator = 0; iterator++) {
  console.log(list[iterator]);
}
```

> 1 error.

## 2.

```js
var list = [99, 98, 97];

for (var iterator = 0; iterator << list.length; iterator++) {
  console.log(list[iterator]);
}
```

> 1 error.

## 3.

```js
var list == [99, 98, 97];

for (var iterator = 0; iterator < list.length; iterator+) {
  console.log(list[iterator]);
}
```

> 2 errors.

## 4.

```js
var list = [99, 98, 97];

for (var iterator = 0; iterator < list.length; iterator++)
  console.log(list[iterator]);
}
```

> 1 error.

# 5.

```js
var list = [99, 98, 97];

for (var iterator = 0; iterator < list.length iterator++) {
  console.log(list[iterator]);
}
```

> 1 error.

# 6.

```js
var list = [99, 98, 97];

for (var iterator = 0; iterator < list length; iterator++) {
  console.log(list[iterator]);
}
```

> 1 error.

# 7.

```js
var list = [99, 98, 97];

for (var iterator = 0; iterator < list.length; iterator++) {
  console.log(list.iterator);
}
```

> 1 error.

# 8.

```js
var list < [99, 98, 97];

if (iterator = 0; iterator < list.length; iterator++) {
  consolelog(list[iterator]);
}
```

> 3 errors.

# 8.

```js
var list = [99, 98, 97];

for (var iterator = 0; iterator = list.length; iterator++;) {
  console.log(list[iterator]);
}
```

> 1 error.

# 9.

```js
function list = [99, 98, 97];

for (var iterator = 0; iterator > list.length; iterator++) {
  console.log(list[iterator]);
};
```

> 2 errors.

# 10.

```js
var list = (99, 98, 97);

for (var iterator == 0; iterator < list.length; iterator++) {
  console.log(list[iterator]);
}
```

> 2 errors.

![](http://ak-hdl.buzzfed.com/static/2015-01/9/4/enhanced/webdr06/anigif_enhanced-13014-1420796486-2.gif)
