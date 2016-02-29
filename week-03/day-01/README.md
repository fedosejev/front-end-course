# Day 1

Questions:

1. [What is a Garbage Collector?](#what-is-a-garbage-collector)
2. [What is closure?](#what-is-closure)
3. [How to create an object?](#how-to-create-an-object)
4. [How to access the properties or methods of an object?](#how-to-access-the-properties-or-methods-of-an-object)
5. [How to update an object?](#how-to-update-an-object)
6. [What is Module Pattern?](#what-is-module-pattern)

Plus:

+ [Problems](#problems)
+ [Learn more](#learn-more)

## Questions

### What is a Garbage Collector?

> The Engine employs a Garbage Collector that comes along and frees up memory once it's no longer in use.

### What is closure?

Remember what a [lexical scope is](https://github.com/frontendeducation/full-time/blob/master/week-02/day-04/README.md#what-is-lexical-scope)?

> Closure is when a function can remember and access its lexical scope even when it's invoked outside its lexical scope.

#### Closure example

+ [Example](http://jsbin.com/nigaso/edit?js,console)
+ [Club example](http://jsbin.com/najuka/edit?js,console)

```js
function createMessage() {
  var message = 'Welcome to the Iron Yard!';
  
  function getMessage() {
    return message;
  }
  
  return {
    getMessage: getMessage
  };
}

var message = createMessage();

console.log(message.getMessage());
```

There are three lexical scopes:
 1. Global scope
 2. Scope of `createMessage` function
 3. Scope of `getMessage` function

Global scope can't reference `message` or `getMessage`. 

#### Without closure

```js
for (var iterator = 1; iterator <= 5; iterator++) {
  setTimeout(function timer() {
    console.log(iterator);
  }, iterator * 1000);
}
```

+ [Example](http://jsbin.com/qihoja/edit?js,console)

#### With closure

```js
for (var iterator = 1; iterator <= 5; iterator++) {
  (function (counter) {
    setTimeout(function timer() {
      console.log(counter);
    }, counter * 1000);
  })(iterator);
}
```

+ [Example](http://jsbin.com/curojo/edit?js,console)

### How to create an object?

```js
var car = {
  make: 'Tesla', // Property
  model: 'Model X',
  color: 'white',
  wheels: 4,
  doors: 5,
  engineSize: 2.0,
  fuelType: 'diesel',
  mileage: 12000,
  additionalOptions: ['navigation', 'winter tyres', 'autopilot'],
  getPrice: function () { // Method
    return '£100,000';
  }
};
```

### How to access the properties or methods of an object?

1. Using dot notation:

  ```js
  car.make;
  ```

  The period is known as the __member operator__.

2. Using square brackets:

  ```js
  car['make'];
  ```

### How to update an object?

```js
car.mileage = 15000;
car['mileage'] = 15000;
```

### What is Module Pattern?

```js
var myTesla = (function TeslaCar() {
  var mileage = 1000;
  var MAKE = 'Tesla';
  var MODEL = 'Model X';
  var color = 'white';
  var WHEELS = 4;
  var DOORS = 5;
  var ENGINE_SIZE = 2.0;
  var FUEL_TYPE = 'diesel';
  var price = 100000;
  
  function getPrice() {
    return '£' + price;
  }
  
  function addMileage(moreMileage) {
    mileage = mileage + moreMileage;
    price = price - parseInt(moreMileage / 3);
    
  }
  
  function getMileage() {
    return mileage;
  }
  
  return {
    price: getPrice,
    mileage: mileage,
    color: color,
    addMileage: addMileage,
    getMileage: getMileage
  };
})();

myTesla.addMileage(10);

console.log(myTesla.getMileage());
console.log(myTesla.price());
```

> Modules require two key characteristics: 1) an outer wrapping function being invoked, to create the enclosing scope 2) the return value of the wrapping function must include reference to at least one inner function that then has closure over the private inner scope of the wrapper.

+ [Example](http://jsbin.com/wehelo/edit?html,js,output)

## Problems

[9 Problems](problems.md)

## Learn more

+ [You Don't Know JS: Scope & Closures](https://github.com/getify/You-Dont-Know-JS/blob/master/scope%20&%20closures/ch5.md)