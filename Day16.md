# ⭐️Day Sixteen (JUL 18 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> Static types & Value types
Static Types:

Static typing is a type system feature where the type of a variable is checked at compile-time. It means that the types of variables are explicitly declared and enforced during the compilation phase. The type of a variable remains fixed throughout its lifetime, and any attempt to assign a value of an incompatible type will result in a compilation error.

Static typing offers several advantages, including:

Early detection of type-related errors during compilation.
Improved code quality and maintainability.
Enhanced tooling support, such as autocompletion and refactoring assistance.
Potential performance optimizations, as the compiler can make assumptions based on the static types.
Examples of programming languages with static typing include Java, C++, C#, and TypeScript.

Value Types:

Value types are a classification of data types based on how they are stored and passed around in memory. In a value type, the actual value is directly stored in the memory location associated with the variable. In other words, when you assign a value type variable to another variable or pass it as a function argument, a copy of the value is made.

Value types have the following characteristics:

The value is stored directly, without the need for additional memory allocations.
Copies of value type variables are independent of each other.
Operations on value types typically involve manipulating the values directly.
Common examples of value types are integers, floating-point numbers, characters, and boolean values. In some programming languages, structures and enumerations are also considered value types.

In contrast to value types, reference types store a reference or pointer to the actual data, rather than the data itself. Changes to one reference variable can affect other references pointing to the same data. Examples of reference types include classes, objects, arrays, and strings.


### ✍️Topic 2 -> lexical scope
In JavaScript, lexical scope refers to the way variable names are resolved in nested functions based on the physical placement of those functions in the source code. The scope of a variable determines where that variable is accessible in your code, and lexical scope is defined by the structure of the code itself.

When a function is defined inside another function, it creates a nested scope. The inner function has access to the variables and functions declared in its own scope, as well as the variables and functions declared in the outer (enclosing) scope. However, the outer scope does not have access to the variables declared inside the inner scope.


### ✍️Topic 3 -> Strict mode
Strict mode in JavaScript is a feature that was introduced in ECMAScript 5 (ES5) to help developers write more secure and robust code. When you enable strict mode in your JavaScript code, it enforces a stricter set of rules and eliminates certain silent errors and unsafe practices that were allowed in the non-strict mode.

To enable strict mode, you simply add the string `'use strict'`; (including the quotes) at the beginning of your JavaScript file or within a function. If used at the top of a script, it applies to the entire script; if used inside a function, it applies only to that specific function and its inner functions.

Here are some of the notable effects and benefits of using strict mode:

Error reporting: In strict mode, certain common coding mistakes that were previously ignored or tolerated are treated as errors. For example, assigning a value to an undeclared variable will throw an error instead of implicitly creating a global variable.

Preventing silent errors: In non-strict mode, some errors might go unnoticed, leading to unexpected behavior. Strict mode helps to catch and raise errors for such cases, making debugging easier.

Eliminating global object leakage: In strict mode, the value of this inside a function is not automatically coerced to the global object when the function is called without a context. This helps to avoid common pitfalls when dealing with this.

Restricted use of reserved keywords: In strict mode, some keywords (such as eval and arguments) cannot be used as variable names, which can prevent potential issues.

Disallowing duplicate parameter names: In strict mode, defining a function with duplicate parameter names is not allowed.


> note -> In JavaScript, a reference error occurs when you try to access a variable or function that is not defined or not accessible in the current scope. This type of error is quite common and can occur for various reasons, such as misspelling a variable name, accessing a variable outside its scope, or trying to use a function that hasn't been declared yet.



## Challenges
- [challenges]()
```javascript
//my solution

```

## Problem
- [problem](https://www.codewars.com/kata/583710ccaa6717322c000105/train/javascript)
```javascript
//my solution
function simpleMultiplication(number) {
    return number % 2 == 0? number*8: number*9;
}
```
