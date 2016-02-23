# Day 2

## Understanding Block Formatting Contexts

Which CSS properties establish new block formatting contexts:
+ The value of `float` is not `none`.
+ The value of `position` is neither `static` nor `relative`.
+ The value of display is `table-cell`, `table-caption`, `inline-block`, `flex`, or `inline-flex`.
+ The value of `overflow` is not `visible`.

---

#### Examples

+ Margin collapse: http://jsbin.com/luxune/edit?html,css,output
+ No margin collapse because of block formatting context: http://jsbin.com/roqaku/edit?html,css,output

---

+ Learn more: http://www.sitepoint.com/understanding-block-formatting-contexts-in-css/
+ W3 documentation: https://www.w3.org/TR/CSS2/visuren.html#block-formatting

## Zero-height container problem for floated elements

+ Problem: http://output.jsbin.com/jehiqumido
+ Source: http://jsbin.com/jehiqumido/edit?html,css

---

+ Learn more: http://learnlayout.com/clearfix.html

## Responsive layouts

To ensure proper rendering and touch zooming, add the viewport meta tag to your `<head>`.

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

+ Learn more: https://developers.google.com/web/fundamentals/design-and-ui/responsive/?hl=en

## What are media queries?

+ [Logic in Media Queries](https://css-tricks.com/logic-in-media-queries/)

#### Examples

+ [Example 1](http://jsbin.com/nugeba/6/edit?html)

> Media queries add no specificity to the selectors they contain, but source order still matters.

## What is Flexbox?

> The Flexbox Layout officially called CSS Flexible Box Layout Module is new layout module in CSS3 made to improve the items align, directions and order in the container even when they are with dynamic or even unknown size. The prime characteristic of the flex container is the ability to modify the width or height of its children to fill the available space in the best possible way on different screen sizes.

+ [A Visual Guide to CSS3 Flexbox Properties](https://scotch.io/tutorials/a-visual-guide-to-css3-flexbox-properties)
+ [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

#### Examples

+ [Example 1](http://jsbin.com/fuduwu/edit?html,output)
+ [Example 2](http://jsbin.com/sedowe/edit?html,output)

## Problems

[4 problems for today](problems.md)

