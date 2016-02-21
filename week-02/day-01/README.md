# Day 1

![](http://tclhost.com/clya4nh.gif)

## What is `display` in CSS?

> The display CSS property specifies the type of rendering box used for an element.

Learn more about `display` property: https://developer.mozilla.org/en-US/docs/Web/CSS/display

## How to hide an element?

`display: none;`

## What is containing block?

> When we specify the positions or dimensions of element boxes, we’re doing so relative to what’s known as the __containing block__.

> The containing block for the root element is called the __initial containing block__.

> The containing block for any other element box is determined by the value of the `position` property for that element.

> If the value of the position property is `static` (the default) or `relative`, the containing block is formed by the edge of the content box of the nearest ancestor element whose `display` property value is one of:

+ `block`
+ `inline-block`
+ Other values

> If the value of the position property is `absolute`, the containing block is the nearest positioned ancestor—in other words, the nearest ancestor whose position property has one of the values `absolute`, `fixed`, or `relative`. The containing block is formed by the __padding edge__ of that ancestor.

+ Example: http://jsbin.com/gasulomomu/edit?html,css,output

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

You can use `:focus` on other HTML elements, for example: http://jsbin.com/hutira/edit?html,css,output

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


