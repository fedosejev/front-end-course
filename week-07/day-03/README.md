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