# ⭐️Day Twelve (JUL 14 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> Prototypes in javaScript
In JavaScript, prototypes are an essential part of the object-oriented programming (OOP) model.

In JavaScript, every object has a prototype, which acts as a blueprint or template for creating other objects. When you access a property or method on an object, JavaScript looks for that property/method directly on the object. If it can't find it, it then checks the object's prototype. If the property/method is still not found, JavaScript continues the search up the prototype chain until it reaches the top-level object, which is usually the Object.prototype.

Prototypes allow objects to inherit properties and methods from other objects, enabling code reuse and creating a hierarchical structure.

```javascript
// Creating a constructor function
function Person(name, age) {
  this.name = name;
  this.age = age;
}

// Adding a method to the prototype
Person.prototype.sayHello = function() {
  console.log("Hello, my name is " + this.name);
};

// Creating an instance of Person
var john = new Person("John", 30);

// Accessing properties and calling methods
console.log(john.name); // Output: John
console.log(john.age); // Output: 30
john.sayHello(); // Output: Hello, my name is John

```

In the example above, we define a constructor function Person that sets the name and age properties on instances of Person. We then add a sayHello method to the Person.prototype, which is shared by all instances of Person.

By using the new keyword, we create a new Person object called john. We can access the properties (name and age) directly on john because they are defined on the object itself. Similarly, we can call the sayHello method on john, even though it is not defined directly on john, but on its prototype.

This way, prototypes allow us to define shared properties and methods that are inherited by all instances of an object, reducing memory usage and promoting code reusability.

I hope this explanation helps! Let me know if you have any further questions.


### ✍️Topic 2 -> `hasOwnProperty()`
the hasOwnProperty method is used to check whether an object has a specific property defined directly on itself, rather than inherited from its prototype chain.

The hasOwnProperty method is a built-in method of the Object prototype. It returns a boolean value indicating whether the object has the specified property as its own property.
```javascript
var person = {
  name: "John",
  age: 30
};

console.log(person.hasOwnProperty("name")); // Output: true
console.log(person.hasOwnProperty("age")); // Output: true
console.log(person.hasOwnProperty("toString")); // Output: false (inherited from Object.prototype)
```
### ✍️Topic 3 -> `this` keyword

the `this` keyword is a special keyword that refers to the context in which a function is executed or an object on which a method is invoked. The value of this is determined dynamically based on how a function is called or a method is accessed.

The behavior of `this` can vary depending on the context:

1. Global scope:

When this is used in the global scope (outside of any function or method), it refers to the global object. In a browser environment, the global object is typically window.

2. Function context:

When this is used within a regular function (not an arrow function), its value is determined by how the function is called.
- If the function is called as a standalone function, this refers to the global object (window in a browser).
- If the function is called as a method of an object, this refers to the object on which the method is invoked.
- If the function is called with the new keyword (constructor invocation), this refers to the newly created object.
- If the function is called using the call() or apply() methods, this is explicitly set to the first argument passed to call() or apply().
3. Method context:

When this is used within an object method, it refers to the object itself—the object on which the method is invoked. The value of this is determined at the time the method is called.

4. Event handlers:

When this is used within an event handler function, it typically refers to the element on which the event occurred.

5. Arrow functions:

In arrow functions, the behavior of the `this` keyword is different compared to regular functions. Arrow functions do not have their own `this` context, and instead, they inherit the `this` value from the surrounding (lexical) scope in which they are defined.


### ✍️Topic 3 -> classes
the `class` keyword is used to define classes, which are a syntactical sugar over the existing prototype-based inheritance model. The `class` syntax provides a more familiar and concise way to create objects and define their behavior.

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  sayHello() {
    console.log("Hello, my name is " + this.name);
  }
}

const john = new Person("John", 30);
console.log(john.name); // Output: John
console.log(john.age); // Output: 30
john.sayHello(); // Output: Hello, my name is John
```

- behavior is shared through inheritance. However, there are cases when inheritance is not the best solution. Inheritance does not work well for unrelated objects like Bird and Airplane. They can both fly, but a Bird is not a type of Airplane and vice versa. For unrelated objects, it's better to use mixins. A mixin allows other objects to use a collection of functions.

```javascript
let flyMixin = function(obj) {
  obj.fly = function() {
    console.log("Flying, wooosh!");
  }
};
```
- immediately invoked function expression or (IIFE) --> execute a function as soon as it is declared.
```javascript
(function () {
  console.log("Chirp, chirp!");
})();
```




## Challenges
Challenges delivered on this [sheet](https://docs.google.com/spreadsheets/d/1JOo_Wqq1tCmrdUjaIRrl-olY0t6SV9RoUXUPoWPvF0Y/edit#gid=0)

## Problem
- [problem](https://www.codewars.com/kata/55a996e0e8520afab9000055/train/javascript)
```javascript
function cookie(x) {
    if (typeof(x) === typeof('hhh')) {
        return 'Who ate the last cookie? It was Zach!'
    } else if (typeof(x) === typeof(1)) {
        return 'Who ate the last cookie? It was Monica!'
    } else {
        return 'Who ate the last cookie? It was the dog!'
    }
}
```
