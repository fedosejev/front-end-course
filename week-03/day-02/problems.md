# Problems

## 1.

How many child nodes and attribute nodes `p` element node has?

```html
<body>
  <div>
    <p id="intro" class="big">
      Welcome <strong>back</strong>!
    </p>
  </div>
</body>
```

## 2.

Given this HTML, add `first` class to the first element in the list and `last` class to the last element in the list using JavaScript:

```html
<ul>
  <li>London</li>
  <li>Paris</li>
  <li>Tokyo</li>
  <li>New York</li>
</ul>
```

## 3.

Replace this:

```html
<div>
  <p id="latest"><strong>Friday</strong> is finally here.</p>
  <p>In addition the weather is sunny today.</p>
</div>
```

With this using JavaScript:

```html
<div>
  <p id="latest">Monday is finally here.</p>
  <p>In addition the weather is sunny today.</p>
</div>
```
## 4.

Write a function `greeting` that takes a greeting message as a parameter and returns a new function that takes a name as a parameter and prints the greeting message with the name.

How to test:

```js
var dayGreeting = greeting('Good morning');
var nightGreeting = greeting('Good evening');

var name = 'Art';

console.log(dayGreeting(name)); // 'Good morning, Art!'
console.log(nightGreeting(name)); // 'Good evening, Art!'
```

## 5.

Build the content of `<body></body>` tag with JavaScript only: http://jsbin.com/tomita/edit?html,outputx

## 6.

Write a function that takes a string as a parameter and returns a reversed version of that string.

Don't use `.reverse()` method.

How to test:

```js
var result = reverse('Hello');

console.log(result); // olleH
```

## 7.

Write a function `isAnagram` which takes in two words as its arguments and returns `true` or `false`. If any of the arguments are missing then `isAnagram` should return `null`.

How to test:

```js
var result;

result = isAnagram('hello', 'olleh');
console.log(result); // true

result = isAnagram('welcome', 'back');
console.log(result); // false

result = isAnagram('london`);
console.log(result); // null
```