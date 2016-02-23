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

---

+ Learn more: https://developers.google.com/web/fundamentals/design-and-ui/responsive/?hl=en

## What are media queries?

+ [Logic in Media Queries](https://css-tricks.com/logic-in-media-queries/)

#### Examples

+ [Example 1](http://jsbin.com/nugeba/6/edit?html)

> Media queries add no specificity to the selectors they contain, but source order still matters.


