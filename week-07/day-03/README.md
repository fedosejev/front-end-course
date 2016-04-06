# Day 3

### How to create React component?

```js
var ReactClass = React.createClass({
  render: function () {
    return React.createElement('h1', { className: 'important' }, 'Introduction');
  }
});

var reactComponentElement = React.createElement(ReactClass);
var parentElement = document.getElementById('react-app');
var reactComponent = ReactDOM.render(reactComponentElement, parentElement);
```

### How to create React component with JSX?

```jsx
var ReactClass = React.createClass({
  render: function () {
    return <h1 className="important">Introduction</h1>;
  }
});

var parentElement = document.getElementById('react-app');
var reactComponent = ReactDOM.render(<ReactClass />, parentElement);
```

+ [List of Tesla cars example without JSX syntax](examples/react-component-without-jsx.html)

```js
var TeslaList = React.createClass({
  render: function () {

    var modelS = React.createElement('li', { className: 'car' }, 'Model S');
    var modelX = React.createElement('li', { className: 'car' }, 'Model X');
    var model3 = React.createElement('li', { className: 'car' }, 'Model 3');

    var liElements = [modelS, modelX, model3];
    var ulElement = React.createElement('ul', null, liElements);

    return ulElement;
  }
});

var reactComponentElement = React.createElement(ReactComponentClass);
var parentElement = document.querySelector('[data-react-app]');
var reactComponent = ReactDOM.render(reactComponentElement, parentElement);
```

+ [List of Tesla cars example with JSX syntax](examples/react-component-with-jsx.html)

```jsx
var TeslaList = React.createClass({
  render: function () {
    return <ul>
      <li className="car">Model S</li>
      <li className="car">Model X</li>
      <li className="car">Model 3</li>
    </ul>;
  }
});

var parentElement = document.querySelector('[data-react-app]');
var reactComponent = ReactDOM.render(<TeslaList />, parentElement);
```
