# Day 3

![](https://alleyhope.files.wordpress.com/2014/05/tumblr_mnenvlkf0o1sqv3nio1_500.gif)

Questions:

+ [Fix errors!](fix-errors.md)
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

+ [Example](http://jsbin.com/tucitubolu/edit?html,console)

### What is a static NodeList?

> When your script updates the page, the NodeList is not updated to reflect the changes made by the script. The methods beginning `querySelector`... return static NodeLists. They reflect the document when the query was made. If the script changes the content of the page, the NodeList is not updated to reflect those changes.

+ [Example](http://jsbin.com/kimegirige/edit?html,console)

### What is DocumentFragment?

> Allows you to create multiple nodes and append them all in once.

+ [Article 1](http://davidwalsh.name/documentfragment)
+ [Example](http://jsbin.com/doquba/edit?html,js,output)

## Problems

1. Draw a DOM tree for this HTML markup:

  ```html
  <li id="message">Welcome to <strong>The Iron Yard</strong> class!</li>
  ```

2. Access the text node and log it's value:

  ```html
  <div>
    <p>JavaScript is pretty powerful.</p>
  </div>
  ```

  _Hint_: use `nodeValue`

3. Log all the text:

  ```html
  <div>
    <p><em>JavaScript</em> is pretty <strong>powerful</strong>.</p>
  </div>
  ```

  _Hint_: use `textContent`

4. Convert all list item text to links:

  ```html
  <ul>
    <li>London</li>
    <li>Paris</li>
    <li>New York</li>
  </ul>
  ```

5. Add class `highlight` to even list items:

  ```html
  <ul>
    <li class="based-in">London</li>
    <li class="visited">San Francisco</li>
    <li>Paris</li>
    <li>Tokyo</li>
    <li class="going-to">New York</li>
  </ul>
  ```

6. Given an array of image URLs, create a web page with a slideshow that updates image every 2 seconds.

  ```js
  var images = [
    'http://valuestockphoto.com/freehighresimages/roast_veg_DSC2834.jpg',
    'http://valuestockphoto.com/freehighresimages/snowy_trees1995.jpg',
    'http://valuestockphoto.com/freehighresimages/nt_alice_springs140362.jpg',
    'http://valuestockphoto.com/freehighresimages/diwali_deepavali_DSC2292.jpg'
  ];
  ```

+ Take a look at [`window.setInterval()`](https://developer.mozilla.org/en-US/docs/Web/API/WindowTimers/setInterval) function.

![](http://i.imgur.com/t8zvc.gif)

## Learn more

+ [The Basics of JavaScript DOM Manipulation](http://callmenick.com/post/basics-javascript-dom-manipulation)
+ [JavaScript DocumentFragment](http://davidwalsh.name/documentfragment)
+ [Document.createDocumentFragment()](https://developer.mozilla.org/en-US/docs/Web/API/Document/createDocumentFragment)
