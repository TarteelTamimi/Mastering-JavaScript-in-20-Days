# ⭐️Day Fifteen (JUL 17 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> 
### ✍️Topic 2 -> 
### ✍️Topic 3 -> 

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
  
}

```

## Problem
- [problem]()
```javascript
// my solution

```
