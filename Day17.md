# ⭐️Day Seventeen (JUL 19 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [ ] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> Hoisting
Hoisting is a behavior in JavaScript where variable declarations and function declarations are moved (or "hoisted") to the top of their containing scope during the compilation phase before the code is executed. This means that you can use variables and functions before they are actually declared in the code.

There are two types of hoisting in JavaScript:

1. Variable Hoisting:
When a variable is declared using `var`, it is hoisted to the top of its function scope or global scope. However, only the declaration is hoisted, not the initialization. The variable is assigned `undefined` during the hoisting phase.

```javascript
console.log(x); // Outputs: undefined
var x = 10;
```

2. Function Hoisting:
Function declarations, unlike variable declarations, are fully hoisted, including both the name and the function body. This means you can call the function before its declaration in the code.

```javascript
myFunction(); // Outputs: "Hello"

function myFunction() {
  console.log("Hello");
}
```
### ✍️Topic 2 -> 
### ✍️Topic 3 ->

## Challenges
- [challenges](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week3-day4-tasks/tasks.md)
```javascript
//my solution

```

## Problem
- [problem](https://www.codewars.com/kata/57e92e91b63b6cbac20001e5/train/javascript)
```javascript
//my solution
function dutyFree(normPrice, discount, hol){
  return Math.floor(hol/(normPrice*discount/100));
}
```
