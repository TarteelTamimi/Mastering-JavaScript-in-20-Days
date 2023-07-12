# ⭐️Day Ten (JUL 12 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [ ] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> Closures
> note-> local memory is deleted when function finish running except for any returned values.

when functions returned other function, we call it **closure**.
```javascript
//example
function createFunction() {
  functon multiplyBy2(num) {
    return num*2;
  }
  return multiplyBy2;
}
const gererateFunction = creataFunction();
const result = generateFunction(3); //6
```
#### Why closures??
when we execute a function, all local data memory will deleted after we exit the function, so closure is to save this data memory.

- calling the function outside of the function call in witch it was defined.

```javascript
function outer() {
  let counter = 0;
  function increamentCounter() {
    counter++;
  }
return increamentCounter;
}
const myNewFunction = outer();
myNewFunction();
myNewFunction();
```
in previous example, we can not access the value of counter unless we run the function `myNewFunction()`

```javascript
//in addition to previous example
const anotherFunction = outer();
anotherFunction();
anotherFunction();
```
the value of counter will be one two one two.

this is because the backpack for `myNewFunction` and the backpack for `anotherFunction` are two different backpacks.

- closures give our function persistent memories and entirely new toolkit for writing professional cade.


## Challenges
- [challenge](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week2-day2-tasks/tasks.md)
```javascript
//chalenge 1

}
```

```javascript
//chalenge 2

}
```

```javascript
//chalenge 3

}
```

```javascript
//chalenge 4

}
```

## Problem
- [problem](https://www.codewars.com/kata/58261acb22be6e2ed800003a/train/javascript)
```javascript
//my solution
class Kata {
  static getVolumeOfCuboid(l, w, h) {
    return l*w*h;
  }
}
```



