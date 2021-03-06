# Problems

## 1.

Draw a DOM tree for this HTML markup:

```html
<li id="message">Welcome to <strong>The Iron Yard</strong> class!</li>
```

Use [draw.io](http://draw.io).

## 2.

Access the text node and log it's value:

```html
<div>
  <p>JavaScript is pretty powerful.</p>
</div>
```

_Hint_: use `nodeValue`

## 3. Log all the text:

```html
<div>
  <p><em>JavaScript</em> is pretty <strong>powerful</strong>.</p>
</div>
```

_Hint_: use `textContent`

## 4.

Convert all list item text to links:

```html
<ul>
  <li>London</li>
  <li>Paris</li>
  <li>New York</li>
</ul>
```

## 5.

Add class `highlight` to even list items:

```html
<ul>
  <li class="based-in">London</li>
  <li class="visited">San Francisco</li>
  <li>Paris</li>
  <li>Tokyo</li>
  <li class="going-to">New York</li>
</ul>
```

## 6.

Given an array of image URLs, create a web page with a slideshow that updates image every 2 seconds.

```js
var images = [
  'http://valuestockphoto.com/freehighresimages/roast_veg_DSC2834.jpg',
  'http://valuestockphoto.com/freehighresimages/snowy_trees1995.jpg',
  'http://valuestockphoto.com/freehighresimages/nt_alice_springs140362.jpg',
  'http://valuestockphoto.com/freehighresimages/diwali_deepavali_DSC2292.jpg'
];
```

+ Take a look at [`window.setInterval()`](https://developer.mozilla.org/en-US/docs/Web/API/WindowTimers/setInterval) function.

## 7.

Write a function that takes a letter and a number as parameters and creates an object with keys where each key is made of a letter + a number from 0 up to a number.

## 8.

Write a function that takes a string as a parameter and returns an object where keys are characters and values are their frequencies.

## 9.

Make sure you can explain what the Bubble Sort is and how it works.