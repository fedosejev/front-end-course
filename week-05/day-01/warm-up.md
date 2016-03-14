# Warm up

## 1.

Write a function that renders a button with a label `Continue`. When user clicks on that button it gets disabled and then a new button is rendered underneath with a label `Finish`. When user clicks on that button it gets disabled and then a message is rendered underneath: `All done!`

## 2.

```js
var message = 'Please sign up.';

var data = {
  message: 'Please enter your email address.'
};

function getMessage() {
  console.log(this.message);
}

var update = {
  data: {
    message: 'Please confirm your email address.'
  }
};
```

Call function `getMessage` 3 times so that it would log the following:

1. `Please sign up.`
2. `Please enter your email address.`
3. `Please confirm your email address.`