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
### ✍️Topic 3 -> 


## Challenges
Challenges delivered on this [sheet](https://docs.google.com/spreadsheets/d/1JOo_Wqq1tCmrdUjaIRrl-olY0t6SV9RoUXUPoWPvF0Y/edit#gid=0)

## Problem
- [problem]()
```javascript

```
