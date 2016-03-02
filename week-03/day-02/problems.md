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

Build the content of `<body></body>` tag with JavaScript only: http://jsbin.com/tomita/edit?html,output

## 5.

Write a function `greeting` that takes a greeting message as a parameter and returns a new function that takes a name as a parameter and prints the greeting message with the name.

How to test:

```js
var dayGreeting = greeting('Good morning');
var nightGreeting = greeting('Good evening');

var name = 'Art';

console.log(dayGreeting(name)); // 'Good morning, Art!'
console.log(nightGreeting(name)); // 'Good evening, Art!'
```