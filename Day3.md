# ⭐️Day Three (JUL 5 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [X] Summarize what I learned

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
> `'Tarteel' == ['Tarteel'] //true`
> `'Tarteel' === ['Tarteel'] //false`
#### Arrays methods 
1. Array.length: return how many elements in the array, ex. `arr.length  //3`
2. Array.includes(element): return whether or not the element exist in the array, ex. `arr.includes(2) //true`
3. Array.pop(): remove the last element in the array, ex. `arr.pop() //the array arr will be [1, 2]`
4. Array.push(element): add or append new elenemt in the end of the array, and return the new length of the array, it change the origin array-in place-, ex. `arr.push(5) //the array arr will be [1, 2, 5]`
5. Array.sort(): sort array elements in alphabatical order
6. Array.join(string): join array elements using string joiner, ex. `arr.join(" * ") //1 * 2 * 5`
7. Array.concat(array): join two different arrays together in one new array, ex. `arr.concat([4, 7]) //it will return[1, 2, 5, 4, 7]`
> if we use `arr.push([4, 7])` instade of `arr.concat([4, 7])` the prevous array will be `[1, 2, 5, [4, 7]]`

#### mutable VS. immutable
- mutable-> we can change it (e.g. arrays)
- immutable always stays the same (e.g. strings)
> in strings we can not change one character using `[ ]`, but we can do it in arrays with elements
```javascript
//example
const family ['father', 'mother', 'child'];
family[2] = 'children';
console.log(family); // ['father', 'mother', 'children']

let name = 'Tarteel';
name[0] = 't';
console.log(name); //Tarteel
```

![note](C:\Users\HP\Desktop\Tarteel\note.png)

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
