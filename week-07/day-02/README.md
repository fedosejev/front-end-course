# Day 2

### How to install React?

```html
<script src="https://fb.me/react-0.14.2.js"></script>
<script src="https://fb.me/react-dom-0.14.2.js"></script>
```

### How to create React element?

```js
var h1Element = React.createElement('h1', { className: 'important' }, 'Welcome');
var parentElement = document.getElementById('react-app');
ReactDOM.render(h1Element, parentElement);
```

Renders:

```html
<h1 class="important" data-reactid=".0">Welcome</h1>
```

+ [Example](http://jsbin.com/qekasu/edit?html,output)

### How to render multiple React elements?

```js
var h1 = React.createElement('h1', { className: 'important', key: 'important' }, 'Introduction');
var p = React.createElement('p', { className: 'content', key: 'content' }, 'Welcome to The Iron Yard!');
var reactFragment = [ h1, p ];
var section = React.createElement('section', { className: 'container' }, reactFragment);
var parentElement = document.getElementById('react-app');

ReactDOM.render(section, parentElement);
```

+ [Example](http://jsbin.com/joguni/edit?html,output)

### How to create React elements of the same type?

Using `React.createFactory`:

```js
var createListItemElement = React.createFactory('li');

var modelS = createListItemElement({ className: 'model-s', key: 'model-s' }, 'Model S');
var modelX = createListItemElement({ className: 'model-x', key: 'model-x' }, 'Model X');
var model3 = createListItemElement({ className: 'model-3', key: 'model-3' }, 'Model 3');

var teslaCars = [modelS, modelX, model3];
var listOfTeslaCars = React.createElement('ul', null, teslaCars);
var parentElement = document.getElementById('react-app');

ReactDOM.render(listOfTeslaCars, parentElement);
```

Using built-in `React.DOM.li` and `React.DOM.ul` factory function:

```js
var modelS = React.DOM.li({ className: 'model-s', key: 'model-s' }, 'Model S');
var modelX = React.DOM.li({ className: 'model-x', key: 'model-x' }, 'Model X');
var model3 = React.DOM.li({ className: 'model-3', key: 'model-3' }, 'Model 3');

var teslaCars = [modelS, modelX, model3];
var listOfTeslaCars = React.DOM.ul(null, teslaCars);
var parentElement = document.getElementById('react-app');

ReactDOM.render(listOfTeslaCars, parentElement);
```

### How to create React elements with JSX?

```jsx
var listOfTeslaCars = <ul>
  <li className="model-s">Model S</li>
  <li className="model-x">Model X</li>
  <li className="model-3">Model 3</li>
</ul>;

var parentElement = document.getElementById('react-app');

ReactDOM.render(listOfTeslaCars, parentElement);
```

[Example](http://jsbin.com/pipuxaz/edit?html,output): notice that you need to import `browser.min.js` file and use `type="text/babel"` on your `<script>` tag.

## References

+ [React Documentation](https://facebook.github.io/react/)
+ [React Element](https://facebook.github.io/react/docs/glossary.html#react-elements)
+ [ReactDOM.render](https://facebook.github.io/react/docs/top-level-api.html#reactdom.render)
+ [React Factories](https://facebook.github.io/react/docs/glossary.html#factories)