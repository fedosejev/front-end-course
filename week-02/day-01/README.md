# Day 1

![](http://tclhost.com/clya4nh.gif)

## How to hide an element?

`display: none;`

## What is containing block?

> When we specify the positions or dimensions of element boxes, we’re doing so relative to what’s known as the __containing block__.

Learn more about containing block: http://reference.sitepoint.com/css/containingblock

## `box-sizing`

1. `content-box` - This is the initial and default value as specified by the CSS standard.
    + [Example](http://jsbin.com/luxoritabo/edit?html,css)
    + [Live](http://output.jsbin.com/luxoritabo)
2. `border-box` - The width and height properties include the padding and border, but not the margin.
    + [Example](http://jsbin.com/xerakocoqi/edit?html,css,output)
    + [Live](http://output.jsbin.com/xerakocoqi)

## What is Pseudo-Classes in CSS?

> Sometimes you need to select parts of a web page that don’t have tags per se, but are nonetheless easy to identify.

### Styles states

##### a:link

> `a:link` selects any link that your guest hasn’t visited yet, while the mouse isn’t hovering over or clicking it. This style is your regular, unused web link.

##### a:visited

> `a:visited` is a link that your visitor has clicked before, according to the web browser’s history.

##### a:hover

> `a:hover` lets you change the look of a link as your visitor moves the mouse over it.

You can use `:hover` on other HTML elements.

##### a:active

> `a:active` lets you determine how a link looks as your visitor clicks. In other words, it covers the brief nanosecond when someone's pressing the mouse button, before releasing it.

##### a:focus

> `:focus` applied when an element has received focus.

Examples: http://jsbin.com/mobasevoxi/edit?html,output

---

+ List of pseudo-classes: https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes

## What is Pseudo-Elements in CSS?

+ `::before` - [example](http://jsbin.com/vaboxor/edit?html,output).
+ `::first-letter` - [example](http://jsbin.com/yelumu/edit?html,output).
+ `::first-line` - [example](http://jsbin.com/puwafu/edit?html,output).

---

+ List of pseudo-elements: https://developer.mozilla.org/en/docs/Web/CSS/Pseudo-elements
+ List of pseudo-classes and pseudo-elements: http://tympanus.net/codrops/css_reference/


