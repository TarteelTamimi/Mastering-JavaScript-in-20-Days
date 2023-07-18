# ⭐️Day Fifteen (JUL 17 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> Introduction

**In javaScript, everything is an object** ---> false 

`false` is not an object
### ✍️Topic 2 -> Primitive Types
In JavaScript, there are five primitive types:

1. Number: Represents numeric values, including integers and floating-point numbers. Examples: 42, 3.14, -10.

2. String: Represents sequences of characters enclosed in single quotes (') or double quotes ("). Examples: 'Hello', "JavaScript".

3. Boolean: Represents a logical value, either true or false, used for conditional statements and comparisons.

4. Undefined: Represents an uninitialized or absent value of a variable that has been declared but not assigned a value. It is a primitive value and there is only one value of undefined.

5. Symbol: Represents a unique identifier. Symbols are often used as property keys in objects to ensure their uniqueness. Symbols are created using the Symbol() function. Example: const mySymbol = Symbol('description').

These primitive types are immutable, which means their values cannot be changed once created. Additionally, they are compared by value, meaning their equality is determined by the actual value they hold rather than any underlying reference.

**In javaScript variables do not hav types, values do**

### ✍️Topic 3 -> typeof operator
the `typeof` operator is used to determine the type of a given value or variable. It returns a string representing the type of the operand.

The syntax of the typeof operator is as follows:

```javascript
typeof operand

console.log(typeof 42); // Output: "number"
console.log(typeof "Hello"); // Output: "string"
```
### ✍️Topic 4 -> special values `NaN`
`NaN` stands for "Not a Number" in JavaScript. It is a special value representing an invalid or unrepresentable numeric result. It is often the result of operations that involve undefined or non-numeric values.

`NaN === NaN //false`
`isNaN("Tarteel") //true`
`Number.isNaN("Tarteel") //false`

> note -> undefined: there is a variable but at the moment it has no value.

> undeclared: it is never been created.

> uninitialized (TDZ): variables declared with `let` and `const` are not yet initialized and cannot be accessed.


## Challenges
- [challenges](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week3-day1-tasks/tasks.md)
```javascript
//Q1
function convertStringToNumber(input) {
  if (typeof input === 'string') {
    return +input;
  } else {
    return {
      value: input,
      type: typeof input
    };
  }
}

//Q2
const checkNaN = (value) => {
  return Number.isNaN(value);
}

//Q3
function isEmptyValue(value) {
  return value === undefined || value === null || value === '';
}

//Q4
function compareObjects(input1, input2) {
  if (typeof input1 !== 'object' || typeof input2 !== 'object') {
    return [input1, input2];
  }

  const keys1 = Object.keys(input1);
  const keys2 = Object.keys(input2);

  if (keys1.length !== keys2.length) {
    return false;
  }

  for (let key of keys1) {
    if (!input2.hasOwnProperty(key) || input1[key] !== input2[key]) {
      return false;
    }
  }

  return true;
}

//Q5
const complexCoercion = (input) => {
  function complexCoercion(input) {
  const type = typeof input;

  if (type === 'number') {
    return Boolean(String(input));
  } else if (type === 'string') {
    return Boolean(input);
  } else if (input === null || input === undefined) {
    return false;
  } else {
    return input;
  }
}

```

## Problem
- [problem](https://www.codewars.com/kata/58bf9bd943fadb2a980000a7/train/javascript)
```javascript
// my solution
function whoIsPaying(name){
  if(name.length <= 2) {
    return [name];
  } else {
    return [name, name.slice(0,2)];
  }
}
```
