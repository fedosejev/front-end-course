# Day 2

+ [Daily warm up](warm-up.md)

Questions:

1. [What is The Document Object Model (DOM)?](#what-is-the-document-object-model-dom)
2. [How to access DOM elements?](#how-to-access-dom-elements)
3. [How to cache DOM queries?](#how-to-cache-dom-queries)

Plus:

+ [Problems](#problems)
+ [Learn more](#learn-more)

## Questions

### What is The Document Object Model (DOM)?

![](http://www.cs.toronto.edu/~shiva/cscb07/img/dom/treeStructure.png)

> As a web browser loads a web page, it creates a model of that page. The model is called a DOM tree and it's stored in the web browser's memory. It consists of four main types of nodes:

1. The `document` node
2. Element nodes
3. Attribute nodes

  > Attribute nodes are not _children_ of the element that carries them; they are _part of_ that element.

4. Text nodes

  > Text nodes cannot have children.

#### Important

> Every element, attribute, and piece of text in the HTML is represented by its own __DOM node__.

> A DOM node _represents_ an element.

### How to access DOM elements?

![](https://www3.ntu.edu.sg/home/ehchua/programming/webprogramming/images/JS_DOMExample.png)

#### Select an individual element node

##### `getElementById()`

+ `document.getElementById()` - [Example](http://jsbin.com/wigetu/edit?html,output)

> Uses the value of an element's id attribute (which should be unique within the page).

##### `querySelector()`

+ `document.querySelector()` - [Example](http://jsbin.com/dolevi/edit?html,output)

> Uses a CSS selector, and returns the first matching element.

#### Select multiple elements (NodeLists)

##### `getElementsByClassName()`

+ `document.getElementsByClassName()` - [Example](http://jsbin.com/celipe/edit?html,output)

> Selects all elements that have a specific value for their `class` attribute.

##### `getElementsByTagName()`

+ `document.getElementsByTagName()` - [Example](http://jsbin.com/quxami/edit?html,output)

> Selects all elements that have the specified tag name.

##### `querySelectorAll()`

+ `document.querySelectorAll()` - [Example](http://jsbin.com/qucetu/edit?html,output)

> Uses a CSS selector to select all matching elements.

#### Traversing between element nodes

##### `parentNode`

> Selects the parent of the current element node.

+ [Example](http://jsbin.com/kajoyey/edit?html,output)

##### `previousSibling`

> Selects the previous sibling from the DOM tree.

> Gecko-based browsers insert text nodes into a document to represent whitespace in the source markup. Therefore a node obtained, for example, using Node.firstChild or Node.previousSibling may refer to a whitespace text node rather than the actual element the author intended to get.

+ [Example](http://jsbin.com/roleni/edit?html,output)

##### [`nextSibling`](https://developer.mozilla.org/en-US/docs/Web/API/Node/nextSibling)

> Selects the next sibling from the DOM tree.

+ [Example](http://jsbin.com/yiximi/edit?html,console,output)

##### `firstChild`

> Select the first child of the current element.

+ [Example](http://jsbin.com/quwomi/edit?html,console)

##### `lastChild`

> Select the last child of the current element.

+ [Example](http://jsbin.com/bimuxu/edit?html,console)

#### Access/update text nodes

##### `nodeValue`

> This property lets you access or update contents of a text node.

+ [Example](http://jsbin.com/palesi/edit?html,console)

#### Work with HTML content

##### `innerHtml`

> Allows access to child elements and text content.

+ [Example](http://jsbin.com/wibase/edit?html,console)

##### `textContent`

> Allows access text content.

+ [Example](http://jsbin.com/sayaru/edit?html,console)

##### [`createElement()`](https://developer.mozilla.org/en-US/docs/Web/API/Document/createElement)

> Lets you create new element node.

+ [Example](http://jsbin.com/ruduwu/edit?html,output)

##### `createTextNode()`

> Lets you create new text node.

+ [Example](http://jsbin.com/ruduwu/edit?html,output)

##### `appendChild()`

> Lets you append child node.

+ [Example](http://jsbin.com/ruduwu/edit?html,output)

##### [`removeChild()`](https://developer.mozilla.org/en-US/docs/Web/API/Node/removeChild)

> Lets you remove child node.

+ [Example](http://jsbin.com/civehu/edit?html,output)

#### Access or update attribute values

##### `className`

> Lets you get or update the value of `class` attribute.

+ [Example](http://jsbin.com/jilepi/edit?html,console)

##### `id`

> Lets you get or update the value of `id` attribute.

+ [Example](http://jsbin.com/makidiw/edit?html,console)

##### `hasAttribute()`

> Checks if attribute exists.

+ [Example](http://jsbin.com/qewoyu/edit?html,console)

##### `getAttribute()`

> Gets attribute's value.

+ [Example](http://jsbin.com/royavi/edit?html,console)

##### `setAttribute()`

> Updates attribute's value.

+ [Example](http://jsbin.com/dureya/edit?html,output)

##### `removeAttribute()`

> Removes attribute.

+ [Example](http://jsbin.com/fekoqi/edit?html,output)

### How to cache DOM queries?

> When people talk about storing elements in variables, they are really storing the location of the elements within the DOM tree in a variable.

> If your script needs to use the same element more than once, you can store the location of the element in a variable.

```js
var importantElement = document.getElementById('important');
```

> That variable stores a __reference__ to the object in the DOM tree.

> DOM queries may return one element, or they may return a NodeList, which is a collection of nodes.

> Element nodes are the DOM representation of an element.

#### `document` Properties

+ `document.title` 
+ `document.lastModified`
+ `document.URL`
+ `document.domain`

```js
var message;

message = '<p>Title: ' + document.title + '</p>';
message = message + '<p>Address: ' + document.URL + '</p>';
message = message + '<p>Last modified: ' + document.lastModified + '</p>';

var footerElement = document.getElementById('footer');
footerElement.innerHTML = message;
```

+ [Example](http://jsbin.com/wehelo/edit?html,js,output)

## Problems

+ [7 problems](problems.md)

## Learn more

+ [Document Object Model](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)
+ [Whitespace in the DOM](https://developer.mozilla.org/en-US/docs/Web/Guide/DOM/Whitespace_in_the_DOM)