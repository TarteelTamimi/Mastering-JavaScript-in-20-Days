# ⭐️Day One (JUL 3 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍ JavaScript principles
#### Execution context
- to run the code of function, we have two parts:
1. **thread of execution**: going through the code line-by-line and run each line.
2. **memory**: save data like strings, arrays and code.
> note-> functions: code we can save (define) and can use later.

> note-> in javaScript we have only one thread of execution.
- we can generalize the function to make it reusable by using parameters, that means that we do not need to decide what dat to run our functionality on until we run the function.
###### (save it ones & use it again and again)
#### First class object 
functions in javaScript = first class object, they can co-exist with and can be treated like any object **functions are objects**.
- so they can be:
1. assigned to variables and properties of other objects.
2. passed as arguments into functions.
3. returned as values from functions.

#### Higher order & callback functions
- Higher order function: the outer function that takes in or passes out a functon.
- Callback function: the function we insert in.

**Higher order & callback functions keep our code DRY (do not repeat yourself)**

#### Pair programming 
when two or more programmers work on the same code, they should avoid:
1. researcher: blocks.
2. stackOverFlow: use cose snippers to fix bug without know how they work.



## Challenges
1. [challenge 1](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-higher-order-functions-map-filter-or-reduce-to-solve-a-complex-problem)
```javascript
const squareList = arr => {
  // Only change code below this line
  const a = arr
  .filter(e  => {
    if (e > 0 && Number.isInteger(e)) {
      return e;
    }
  })
  .map(e => {
    return e*e;
  })
  return a;
  // Only change code above this line
};


const squaredIntegers = squareList([4, 5.6, -9.8, 3.14, 42, 6]);
console.log(squaredIntegers); 

```

2. [challenge 2](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/apply-functional-programming-to-convert-strings-to-url-slugs)
```javascript
// Only change code below this line
function urlSlug(title) {
  return title
    .split(" ")
    .filter(substr => substr !== "")
    .join("-")
    .toLowerCase();
}

// Only change code above this line
console.log(urlSlug("A Mind Needs Books Like A Sword Needs A Whetstone")) 
```


## Problem
- [problem](https://www.codewars.com/kata/5ab6538b379d20ad880000ab/train/javascript)
```javascript
const areaOrPerimeter = function(l , w) {
  if (l==w) {
    return l*w
  } else {
    return 2*l + 2*w;
  }
};
```



