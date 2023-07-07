# ⭐️Day Five (JUL 7 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> functions
> values are things,
> vatiables point to things,
> functions do things.
- we have two perspective when we talk about functions:
1. creation:
```javascript
function funName(paras) {
 //the body
}
```
2. using:
```javascript
funName(args);
```
#### parameters & arguments 
parameters are the values that the function need to work, while the arguments are the actual values passed to the function.

> note -> `NaN` stand for not a number, it happend in many cases like: `1 + undefined` or `10 / 0`.
- a return statement specifies the function's output value, and it exit the function.
> note -> evert function in javaScript should return a value, if the function does not have a return statement it returns `undefined`.

other way to declare a function:
```javaScript
const funName = function(paras) {
 //the body
}
```

#### arrow function 
we use fat arrow `=>` to create an unnamed function without much code
```javascript
(x, y) => x + y;
```

### ✍️Topic 2 -> scope of variables
scope cares about where we declare our variables, and determines where it are "in play".
> note -> global is the widest scope

within each scope, you can access variables declared in a wider scope (e.g. global scope), but not those declared in a narrower scope (e.g. function scope).
- `let` has a block scope
```javascript
{
 let x = "Hi javaScript"
}
console.log(x) //this will return error
```


## Challenges
- [challenge 1]()
```javascript

```

## Problem
- [problem]()
```javascript

```
