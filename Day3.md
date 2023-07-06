# ⭐️Day Three (JUL 5 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [ ] Summarize what I learned

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
> `let a`, the value of `a` will be `undefined`.
- single equals `=` uses for assignment
- javaScript is dynamic typing (do not care about the data type of the variable)
> we use camelCase to name variables in javaScript.
> variable is not a box that contain value, it is points to a value.
- expressions ---> creat values / assignment ---> creats a reference
#### Statements VS. Expressions
- statements tell javaScript what to do, ex. `let ten = 6 + 4;`
- expressions ask javaScript what is the value, ex. `document.title`
  
### ✍️Topic 2 -> arrays
- arrays let us keep multiple values together in a single colledtion.
- to declare an array `const arr = [1, 2, 3];`
- we can store any type of data in array `const arr = [10, "Tarteel", false];`
- as strings, each element in arrays has an index `arr[0]`
#### Arrays methods 
1. .length: return how many elements in the array `arr.length  //3`


### ✍️Topic 3 -> 
### ✍️Topic 4 -> 

## Challenges
- [challenge 1](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-data-structures/copy-array-items-using-slice)
```javascript
// my solution
function forecast(arr) {
  // Only change code below this line
  let newarr = arr.slice(2, 4);

  return newarr;
}

// Only change code above this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));
```

- [challenge 2](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-data-structures/combine-arrays-with-the-spread-operator)
```javascript
// my solution
function spreadOut() {
  let fragment = ['to', 'code'];
  let sentence = ['learning', ...fragment, 'is', 'fun']; // Change this line
  return sentence;
}

console.log(spreadOut());
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
