# Day 4

### Warm up

1. http://jsbin.com/zoboje/edit?js,output
2. [](warm-up.md)

![](https://i.imgur.com/c1HtJvR.gif)

Questions:

+ [What is an event?](#what-is-an-event)
+ [How to trigger JavaScript code when an event occurs?](#how-to-trigger-javascript-code-when-an-event-occurs)
+ [How to bind an event to an element?](#how-to-bind-an-event-to-an-element)
+ [How to pass a parameter to event listener?](#how-to-pass-a-parameter-to-event-listener)
+ [How events flow?](#how-events-flow)
+ [What is an event object?](#what-is-an-event-object)
+ [How to delegate event?](#how-to-delegate-event)
+ [How to run JavaScript function when the web page has finished loading?](#how-to-run-javascript-function-when-the-web-page-has-finished-loading)

Plus:

+ [Problems](#problems)
+ [Learn more](#learn-more)

## Questions

### What is an event?

> An event is a mechanism for a web browser to say that something has happened.

#### UI events

+ `load` - web page has finished loading.
+ `unload` - web page is unloading.
+ `error` - JavaScript error or asset doesn't exist.
+ `resize` - web browser window resize.
+ `scroll` - user has scrolled up and down the web page.

#### Keyboard events

+ `keydown` - user presses a key.
+ `keyup` - user releases a key.

#### Mouse events

+ `click` - user presses and releases a button over the same element.
+ `mouseover` - user moves the mouse over an element.

[More events](https://developer.mozilla.org/en-US/docs/Web/Events)

> Events can be __fired__ or __raised__.

> Events __trigger__ a function or script.

### How to trigger JavaScript code when an event occurs?

1. Select the __element__ node(s) you want the script to respond to.
2. Indicate which __event__ on the selected node(s) will trigger JavaScript code, i.e. __bind__ an event to a DOM node.
3. State the __code__ you want to run when the event occurs.

### How to bind an event to an element?

1. HTML event handlers.
2. DOM event handlers.
3. DOM event listeners.

#### HTML event handlers

**WARNING: bad practice - don't do that!**

```html
<button onclick="doSomething()">Do something</button>
```

`onclick` attribute indicates that when user clicks on that button - `doSomething` function will be triggered.

+ [Example](http://jsbin.com/widiza/edit?html,js,console,output)

#### DOM event handlers

+ Advantage: all modern web browsers understand this way of creating an event handler.
+ Disadvantage: you can attach only one function to each event handler.

```js
element.onevent = functionName;
```

+ [Example](http://jsbin.com/tequfu/edit?html,js,console,output)

#### DOM event listeners

**Recommended!**

+ Advantage: can trigger more than one function at a time.
+ Disadvantage: not supported in older web browsers.

```js
element.addEventListener('event', functionName, boolean);
```

+ [Example](http://jsbin.com/vehobo/edit?html,js,console,output)

### How to pass a parameter to event listener?

We can't pass a parameter `'important'` to `doSomething` event listener function:

```js
element.addEventListener('click', doSomething, eventDirection);
```

We need to wrap our `doSomething` function into `handleEvent` function:

```js
element.addEventListener('click', function handleEvent() {
  doSomething('important');
}, false);
```

+ [Example](http://jsbin.com/juduki/edit?html,js,console,output)

### How events flow?

> HTML elements nest inside other elements. If you click on a link, you will be clicking on its parent elements as well.

![](http://adaptivewebdesign.info/1st-edition/read/images/Ch4-2.jpg)

#### What is _event bubbling_?

> The event starts at the __most specific__ node and _flows outwards_ to the __least specific__ one.

> This is a default type of event flow.

For example:

```html
<section>
  <ul>
    <li>
      <a href="http://artemij.com">My website</a>
    </li>
  </ul>
</section>
```

When you click on `My website` link, JavaScript can trigger events on:

1. The `<a>` element
2. The `<li>` element
3. The `<ul>` element
4. The `<section>` element
5. The `<body>` element
6. The `<html>` element
7. The `document` object

#### What is _event capturing_?

> The event starts at the __least specific__ node and _flows inwards_ to the __most specific__ one.

#### How to choose bubbling or capturing direction?

```js
addEventListener(eventType, eventListener, eventDirection);
```

Provide boolean value for `eventDirection` parameter:
+ `true` - capturing phase.
+ `false` - bubbling phase (often used by default).

[Example](http://jsbin.com/jodelo/edit?html,js,console,output)

### What is an event object?

> When an event occurs, the event object tells you information about the event, and the element it happened upon.

> The event object is passed to any function that is the event handler or listener.

#### Properties

+ `target` - The target of the event, i.e. the most specific element interacted with.
  + [Example](http://jsbin.com/heboha/edit?html,js,console,output)
+ `type` - Type of the event that was fired.
  + [Example](http://jsbin.com/zuqege/edit?html,js,console,output)

#### Methods

+ `preventDefault()` - Cancel default behaviour of the event.
  + [Example](http://jsbin.com/vonusa/edit?html,js,output)
+ `stopPropagation()` - Stops the event from bubbling or capturing any further.
  + [Example](http://jsbin.com/socepu/edit?html,js,console,output)

#### How to pass an event object __and__ other arguments to your event listener function?

+ [Example](http://jsbin.com/bisace/edit?html,js,console,output)

### How to delegate event?

> Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element.

+ [Example](http://jsbin.com/gofoyu/6/edit?html,css,js,output)

### How to run JavaScript function when the web page has finished loading?

+ Listen to `load` event.

> The load event fires at the end of the document loading process. At this point, all of the objects in the document are in the DOM, and all the images, scripts, links and sub-frames have finished loading.

+ [Example](http://jsbin.com/jeseba/edit?js,output)

## Problems

+ [Project](../project.md)

![](http://www.conceptart.org/forums/attachment.php%3Fattachmentid%3D1916307%26d%3D1392949853)

## Learn more

+ [List of all events](https://developer.mozilla.org/en-US/docs/Web/Events)
+ [How JavaScript Event Delegation Works](http://davidwalsh.name/event-delegate)
+ [Load event](https://developer.mozilla.org/en/docs/Web/API/GlobalEventHandlers/onload)
