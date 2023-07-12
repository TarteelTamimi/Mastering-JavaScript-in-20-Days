# ⭐️Day Seven (JUL 9 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [ ] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> asynchronuous coding
`console.log('Hello')` is vary quick, and javaScript can usually run straight through our program "synchronously" (e.g. one thing at a time), so we need way in javaScropt that allows us to do multiple taskes together witch called **asynchronous**. 
#### fetching data
`fetch()` is a built-in function witch let us use javaScript to load data from APIs, ex. `fetch('https://getemoji.com/');`, and it returns a **promise**.
> note -> JSON stands for javaScript object notation.
#### promise
promises promise us that it will give us the data we want, but it does not hava it yet.
- promises can be in three states:
1. pending: still waiting for the value.
2. fulfilled (resolved): got the value successfully.
3. rejected: could not get the value.

#### await 
await let us tell javaScript to stop and wait for an asynchronous operation to finish.
```javascript
//example
let response = await fetch("URL")
// it will wait for it to resolve before continuing with our code.
```
- `response.json()` to parse the body of response as a JSON object, and will return another promise, so we will use await again.
```javascript
let response = await fetch("URL");
let body = await response.json();
```

### ✍️Topic 2 -> Destructing 
destructing is a fancy way of declaring multiple variables at one, by "extracting" values from an object with their properties.
```javascript
const spices = {anme: "Emma", nickname: "Baby"};
let {name, nickname} = spices;
```
and we can apply it on arrays.

- the order does not matter in objects destructuring, but it matter in array destructuring.

## Challenges
- [challenge ](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week1-day5-task/task.md)
```javascript
//my solution
<!DOCTYPE html>
<html>
<head>
  <title>Alive Character List</title>
  <link rel="stylesheet" href="./styles.css">
</head>
<body>
  <h1>Alive Character List</h1>
  <ul id="characterList"></ul>

  <script src="./script.js"></script>
</body>
</html>
}
```

## Problem
- [problem](https://www.codewars.com/kata/57a0556c7cb1f31ab3000ad7/train/javascript)
```javascript
//my solution
function makeUpperCase(str) {
  return str.toUpperCase();
}
```


