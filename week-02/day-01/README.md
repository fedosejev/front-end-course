# Day 1

![](http://tclhost.com/clya4nh.gif)

## `box-sizing`

1. `content-box` - This is the initial and default value as specified by the CSS standard.
    + [Example](http://jsbin.com/luxoritabo/edit?html,css)
    + [Live](http://output.jsbin.com/luxoritabo)
2. `border-box` - The width and height properties include the padding and border, but not the margin.
    + [Example](http://jsbin.com/xerakocoqi/edit?html,css,output)
    + [Live](http://output.jsbin.com/xerakocoqi)

## What is Pseudo-Classes in CSS?

> Sometimes you need to select parts of a web page that don’t have tags per se, but are nonetheless easy to identify.

#### Styles for links

##### a:link

> `a:link` selects any link that your guest hasn’t visited yet, while the mouse isn’t hovering over or clicking it. This style is your regular, unused web link.

##### a:visited

> `a:visited` is a link that your visitor has clicked before, according to the web browser’s history.

##### a:hover

> `a:hover` lets you change the look of a link as your visitor moves the mouse over it.

You can use `:hover` on other HTML elements.

##### a:active

> `a:active` lets you determine how a link looks as your visitor clicks. In other words, it covers the brief nanosecond when someone's pressing the mouse button, before releasing it.

+ `:focus`

Examples: http://jsbin.com/tumoku/edit?html,output

### What is Pseudo-Elements in CSS?

+ `:before` - [example](http://jsbin.com/lixeso/edit?html,output).
+ `:first-letter` - [example](http://jsbin.com/qiwohe/edit?html,output).
+ `:first-line` - [example](http://jsbin.com/qogagu/edit?html,output).
