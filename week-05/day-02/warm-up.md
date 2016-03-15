# Warm up :fire: :muscle:

![](http://www.blogcdn.com/www.pawnation.com/media/2013/09/kitten-cant-control-his-feet---imgur.gif)

## Let's explore!

Put this line in Chrome's console:

```js
var message = new SpeechSynthesisUtterance('How\'s everyone doing this morning? Welcome to the daily warm up!'); message.lang = 'en-US'; window.speechSynthesis.speak(message);
```

+ [Getting Started with the Speech Synthesis API](http://blog.teamtreehouse.com/getting-started-speech-synthesis-api)

## 1.

Write a function `push()` that adds an element to an array.

It accepts two parameters:

1. Array, e.g.: `['a', 'b', {}]`
2. Value, e.g.: `[]`

It returns an array with that value added at the end.

#### How to test

```js
push(['a', 'b', {}], []);
```

Retuns:

```js
['a', 'b', {}, []]
```

## 2.

Write a function `pop()` that takes an array and returns it's last item.

#### How to test

```js
pop(['a', 'b', {}]);
```

Retuns:

```js
{}
```

### 3.

Given this document:

```html
<div>
  <ul>
    <li data-city="london">London</li>
    <li data-city="los-angeles">Los Angeles</li>
    <li data-city="san-francisco">San Francisco</li>
  </ul>
</div>
```

And this data:

```js
var cities = {
  'london': {
    name: 'London',
    country: 'UK'
  },
  'los-angeles': {
    name: 'Los Angeles',
    country: 'US'
  },
  'san-francisco': {
    name: 'San Fracisco',
    country: 'US'
  }
};
```

Write a function `removeCity()` takes a parameter that represents a city and removes it from both: the DOM and `cities` object.

It returns `true` if removed successfully or `false` if failed to remove.

#### How to test

```js
removeCity('london'); // Returns `true`.
removeCity('paris'); // Returns `false`.
removeCity(); // Returns `false`
```

+ [Using data attributes](https://developer.mozilla.org/en/docs/Web/Guide/HTML/Using_data_attributes)
