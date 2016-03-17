# Day 3

:fire: [Warm up](warm-up.md) :fire:

![](http://rack.1.mshcdn.com/media/ZgkyMDEzLzA3LzA1L2NkL0FuY2hvcm1hbi42NjJkYS5naWYKcAl0aHVtYgkxMjAweDk2MDA-/074dbca9/1c0/Anchorman.gif)

Questions:

+ [How to update DOM elements with jQuery?](#)
+ [How to create new DOM elements with jQuery?](#)
+ [How to insert new DOM elements with jQuery?](#)
+ [How to get and set attributes with jQuery?](#)
+ [How to get and set CSS rules with jQuery?](#)
+ [How to loop through elements with jQuery?](#)
+ [How to add event listeners with jQuery?](#)
+ [How to delegate event handling with jQuery?](#)
+ [How to create effects with jQuery?](#)
+ [How to traverse the DOM with jQuery?](#)
+ [How to create complex UI widgets?](#)
+ [How to create a map?](#)

Plus:

+ [Problems](#problems)
+ [Learn more](#learn-more)

## Questions:

### How to update DOM elements with jQuery?

#### `.html()` and `.text()`

+ [`.html()`](http://api.jquery.com/html/)
+ [`.text()`](http://api.jquery.com/text/)

[Example](http://jsbin.com/hofone/edit?html,output)

#### `.remove()` and `.replaceWith()`

+ [`.replaceWith()`](http://api.jquery.com/replacewith/)
+ [`.remove()`](http://api.jquery.com/remove/)

[Example](http://jsbin.com/wecuy/edit?html,output)

### How to create new DOM elements with jQuery?

```js
var santaCruz = $('<li data-city-name="santa-cruz" class="popular">Santa Cruz</li>');
```

### How to insert new DOM elements with jQuery?

#### `.before()`

```js
$('[data-city-name="los-angeles"]').before(santaCruz);
```

#### `.after()`

```js
$('[data-city-name="santa-cruz"]').after(boston);
```

[Example](http://jsbin.com/belayi/edit?html,output)

#### `.prepend()`

```js
// Insert content inside the selected element(s)
$('[data-city-name="london"]').prepend('<small>Popular: </small>');
```

#### `.append()`

```js
// Insert content after the selected element(s)
$('[data-city-name="london"]').append('<small> (UK)</small>');
```

[Example](http://jsbin.com/pexafox/edit?html,output)

### How to get and set attributes with jQuery?

#### `.attr()`

```js
// Select the first element without data-city-name attribute and set that attribute
$('li:not([data-city-name])').first().attr('data-city-name', 'new-york');
```

Take a look at `attr.html`.

#### `.addClass()`

```js
$('[data-city-name="los-angeles"]').addClass('popular');
```

[Example](http://jsbin.com/zafune/edit?html,output)

#### `.removeClass()`

```js
$('[class="popular"]').removeClass('popular');
```

[Example](http://jsbin.com/futobi/edit?html,output)

### How to get and set CSS rules with jQuery?

#### `.css()`

Get:

```js
$('[data-city-name="london"]').css('font-size');
```

Set:

```js
$('li').css('text-transform', 'uppercase');
```

Take a look at `css.html`.

### How to loop through elements with jQuery?

```js
$('li').each(function () {
  $(this).addClass('city');
});
```

[Example](http://jsbin.com/tiruka/edit?html,output)

### How to add event listeners with jQuery?

```js
$('li').on('click', function () {
  $(this).removeClass('city');
});
```

[Example](http://jsbin.com/rixogu/edit?html,output)

### How to delegate event handling with jQuery?

```js
$('ul').on('click', 'li', function () {
  $(this).removeClass('city');
});
```

[Example](http://jsbin.com/begaqa/edit?html,output)

### How to create effects with jQuery?

+ `.show()`
+ `.hide()`
+ `.toggle()`
+ `.fadeIn()`
+ `.fadeOut()`
+ `.slideUp()`
+ `.slideDown()`

### How to traverse the DOM with jQuery?

+ `.find()`
+ `.parent()`
+ `.children()`
+ `.siblings()`
+ `.next()`
+ `.prev()`

## Learn more

+ [jQuery](https://jquery.com/)
