# ⭐️Day Three (JUL 5 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> expressions & variables
- values + operators to evaluate a value
- there are three ways to declare a variables in javaScript: var, let and const.
  we can differentiate between them interms of
1. scope,
2. redecleration,
3. reassignment,
4. hoisting,
    as follow:
    + var-> functional scope, redecleration✅, reassignment✅, hoisting✅.
    + let-> block scope, redecleration❎, reassignment✅, hoisting❎.
    + const-> block scope, redecleration❎, reassignment❎, hoisting❎.
> `let a` the value of `a` will be `undefined`.
- single equals `=` uses for assignment
- javaScript is dynamic typing (do not care about the data type of the variable)
> we use camelCase to name variables in javaScript.
> variable is not a box that contain value, it is points to a value.
- expressions ---> creat values / assignment ---> creats a reference
#### Statements VS. Expressions
- statements tell javaScript what to do, ex. `let ten = 6 + 4;`
- expressions ask javaScript what is the value, ex. `document.title`
  
### ✍️Topic 2 -> 
### ✍️Topic 3 -> 
### ✍️Topic 4 -> 

## Challenges
- [challenge 1]()
```javascript
// my solution

```


## Problem
- [problem](https://www.codewars.com/kata/570a6a46455d08ff8d001002/train/javascript)
```javascript
// my solution
function noBoringZeros(n) {
  if (n==0) {
    return n;
  } else {
    while (n%10==0) {
      n/=10;
    }
    return n;
  }
}
```
