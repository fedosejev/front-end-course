# Day 1

:fire: [Warm up](warm-up.md) :fire:

Questions:

+ [What is `this`?](#)
+ [What is call-site?](#)
+ [How to attach event listener to a jQuery object?](#)
+ [How to create DOM nodes using jQuery?](#)

Plus:

+ [Problems](#problems)
+ [Learn more](#learn-more)

## Questions

### What is `this`?

> Allows to reuse function against multiple context objects, rather than needing a separate version of the function for each object.

Without `this`:

```js
var instructor = {
  name: 'Art'
};

var student = {
  name: 'John'
};

function whatIsYourName(contextObject) {
  console.log(contextObject.name);
}

whatIsYourName(instructor);
whatIsYourName(student);
```

+ [Example](http://jsbin.com/yomoku/edit?js,console)

With `this`:

```js
var instructor = {
  name: 'Art'
};

var student = {
  name: 'John'
};

function whatIsYourName() {
  console.log(this.name);
}

whatIsYourName.call(instructor);
whatIsYourName.call(student);
```

+ [Example](http://jsbin.com/mejoxu/edit?js,console)

> Implicitly passing along an object reference is cleaner than passing context around as an explicit parameter.

> `this` is not an author-time binding but a runtime binding.

+ [Read this](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20&%20object%20prototypes/ch1.md#whats-this)

### What is call-site?

> The location in code where a function is called.

+ Take a look at `call-site.html` file in Chrome with developer tools turned on.

### How to determinte call-site?

> 4 rules.

#### 1. Default Binding

```js
function logName() {
  console.log(this.name);
}

var name = 'Art';

logName();
```

+ [Example](http://jsbin.com/leniya/edit?js,console)

> Variables declared in the global scope (`var name = 'Art';`) are synonymous with global-object properties of the same name (`window.name = 'Art';`).

#### 2. Implicit Binding

```js
function logName() {
  console.log(this.name);
}

var person = {
  name: 'Art',
  logName: logName
};

person.logName();
```

+ [Example 1](http://jsbin.com/jasexi/edit?js,console)
+ [Example 2](http://jsbin.com/zipogam/edit?js,console)
+ [Example 3](http://jsbin.com/cojela/edit?js,console)

#### 3. Explicit Binding

```js
function logName() {
  console.log(this.name);
}

var person = {
  name: 'Art',
  logName: logName
};

logName.call(person);
```

+ [Example](http://jsbin.com/letoye/edit?js,console)


#### Hard Binding

```js
function logName() {
  console.log(this.name);
}

var instructor = {
  name: 'Art',
  logName: logName
};

var student = {
  name: 'John',
  logName: logName
};

var logInstructorName = logName.bind(instructor);

logInstructorName.call(student);
```

+ [Example](http://jsbin.com/sogafeq/edit?js,console)

#### 4. `new` Binding

> `new` operator.
> Construction calls _of_ functions.

```js
function person(name) {
  this.name = name;
}

var art = new person('Art');

console.log(art.name);
```

+ [Example](http://jsbin.com/lomeco/edit?js,console)

> When a function is invoked with new in front of it, otherwise known as a constructor call, the following things are done automatically:

1. a brand new object is created (aka, constructed) out of thin air
2. the newly constructed object is [[Prototype]]-linked
3. the newly constructed object is set as the this binding for that function call
4. unless the function returns its own alternate object, the new-invoked function call will automatically return the newly constructed object.

##### Order of precedence?

1. `new` Binding
2. Explicit Binding
3. Implicit Binding
4. Default Binding

[Read this](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20&%20object%20prototypes/ch2.md#review-tldr)

## Learn more

+ [You Don't Know JS: this & Object Prototypes](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20&%20object%20prototypes/ch1.md)
+ [Understanding JavaScript Function Invocation and "this"](http://yehudakatz.com/2011/08/11/understanding-javascript-function-invocation-and-this/)