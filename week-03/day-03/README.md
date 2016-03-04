# Day 3

+ [Fix errors!](fix-errors.md)

![](https://alleyhope.files.wordpress.com/2014/05/tumblr_mnenvlkf0o1sqv3nio1_500.gif)

Questions:

+ [What is a NodeList?](#what-is-a-nodelist)
+ [What is a live NodeList?](#what-is-a-live-nodelist)
+ [What is a static NodeList?](#what-is-a-static-nodelist)
+ [What is DocumentFragment?](#what-is-documentfragment)

Plus:

+ [Problems](#problems)
+ [References](#references)

## Questions

### What is a NodeList?

> NodeList is a collection of nodes.

The following methods will returns a NodeList:

+ `getElementsByClassName()`
+ `getElementsByTagName()`
+ `querySelectorAll()`

### What is a live NodeList?

> When your script updates the page, the NodeList is updated at the same time. The methods beginning `getElementBy`... return live NodeLists. They are typically faster to generate than static NodeLists.

+ [Example](http://jsbin.com/lovodac/edit?html,console)

### What is a static NodeList?

> When your script updates the page, the NodeList is not updated to reflect the changes made by the script. The methods beginning `querySelector`... return static NodeLists. They reflect the document when the query was made. If the script changes the content of the page, the NodeList is not updated to reflect those changes.

+ [Example](http://jsbin.com/jonusa/edit?html,console)

### What is DocumentFragment?

> Allows you to create multiple nodes and append them all in once.

+ [Article 1](http://davidwalsh.name/documentfragment)
+ [Example](http://jsbin.com/doquba/edit?html,js,output)

## Problems

[9 problems](problems.md)

![](http://i.imgur.com/t8zvc.gif)

## Learn more

+ [The Basics of JavaScript DOM Manipulation](http://callmenick.com/post/basics-javascript-dom-manipulation)
+ [JavaScript DocumentFragment](http://davidwalsh.name/documentfragment)
+ [Document.createDocumentFragment()](https://developer.mozilla.org/en-US/docs/Web/API/Document/createDocumentFragment)
