# Day 2

![](http://33.media.tumblr.com/tumblr_m4m07q2EVu1rpkyvk.gif)

:fire: [Warm up](warm-up.md) :fire:

Questions:

+ [What is jQuery?](#)
+ [How to install jQuery?](#)
+ [How to use jQuery?](#)

Plus:

+ [Problems](#problems)
+ [Learn more](#learn-more)

## Questions

### What is jQuery?

> jQuery is a JavaScript library that lets you query elements using CSS-style selectors and then do something with the elements using jQuery methods.

### How to install jQuery?

Put into `<head>` of your HTML file:

```html
<script src="http://code.jquery.com/jquery-2.1.4.min.js"></script>
```

### How to use jQuery?

```js
jQuery('selector');
```

Or:

```js
$('selector');
```

+ `$()` is a shorthand version of `jQuery()`.
+ `$` is a valid function/variable name in JavaScript. [Example](http://jsbin.com/bedice/edit?js,console).

#### Example

__Step 1__: Select DOM elements.

```js
$('li.new');
```

Returns jQuery object that represents all of the `li` elements with a class of `new`.

> `jQuery()` or `$()` function has one parameter: a CSS-style selector.

+ [jQuery Selectors](https://dzone.com/refcardz/jquery-selectors)

__Step 2__: So something with selected elements.

```js
$('li.new').addClass('exclusive');
```

Quiz: find _member operator_.

### How to check if page is ready with jQuery?

```js
$(document).ready(function () {
  // Your code goes here
});
```

Or a shortcut version:

```js
$(function () {
  // Your code goes here
});
```

+ [Example](http://jsbin.com/cogevi/edit?html,js,output)
+ Compare DOM manipulation [without jQuery](http://jsbin.com/gofoyu/6/edit?html,css,js,output) and [with jQuery](http://jsbin.com/qanaxi/edit?html,css,js,output).
+ No need to loop through array of nodes. [Example](http://jsbin.com/vifece/edit?html,css,js,output).
+ Can chain methods. [Example](http://jsbin.com/zutiti/edit?html,js,output).

## Problems

1. Create a copy of Photo Gallery web app - use jQuery instead of native DOM manipulation.

## Learn more

+ [DOMContentLoaded](https://developer.mozilla.org/en-US/docs/Web/Events/DOMContentLoaded)
+ [jQuery API](http://api.jquery.com/)
+ [jQuery Selectors](https://dzone.com/refcardz/jquery-selectors)
+ [You Might Not Need jQuery](http://youmightnotneedjquery.com/)
