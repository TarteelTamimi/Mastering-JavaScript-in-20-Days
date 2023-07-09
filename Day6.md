# ⭐️Day Six (JUL 8 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> conditionals
- if statement let us execute code under a certain condition, ex.
```javascript
if (3>1) {
  console.log('Three greater than one');
}
```
code in the block only runs if the (condition) is true.
- we can use `else` to run other code if (condition) is false
```javascript
if (name == "Tarteel") {
  console.log('we find her!!!!');
} else {
  console.log('ohhh she is lost :(');
}
```
- we can chain `else` and `if` blocl=ks to account for multiple conditions
```javascript
if (num > 0 ) {
  console.log('positive');
} else if (num < 0) {
  console.log('negative');
} else {
  console.log('zero');
}
```
> if we pass a non empty string to the `if` statement then javaScript will consider it as truthy, the `0` is falsy, any other number is truthy, an array whether ro not is empty is truthy (objects are truthy), `null` and `undefined` are falsy.

### ✍️Topic 2 -> boolean (logical) operaters
1. `!` negates aboolean, `!true = false`
2. `&&` if we care about the truthiness of more than one value
3. `||` if we care about the truthiness ot at least one condition

#### conditional ternary operator 
it is a quick way of writting if-else statements in javaScript (condition? valueIfTrue: valueIfFalse)
```javascript
a > b?"a greater than b":"b greater than or equals a";
```
is equivalent to 
```javascript
if (a>b) {
  return "a greater than b";
} else {
  return "b greater than or equals a";
}
```

### ✍️Topic 3 -> loops
- loops let us run the same chunk of code multiple times (aka iteration)
```javascript
for (let count=1; count<=10; count++) {
  console.log(count);
}
```
- for ... of let us more easily iterate over items in a collection, we can use it for arrays and strings because they are **iterables**.
```javascript
for (let i=0; i<arr.length; i++) {
  console.log(arr[i]);
}
```
is equivalent to 
```javascript
for (let x of arr) {
  console.log(x);
}
```

#### while loop
while loop let us run a chunk of code over & over if a condition is true.
```javascript
//example
while (4>1) {
  console.log('Hiii');
}
```


### ✍️Topic 4 -> map & filter
map and filter are methods also let us process all the items in an array.
#### map
it calls a function on each item in an array to create a new array.
```javascript
const numbers = [65, 44, 12, 4];
const newArr = numbers.map(myFunction)

function myFunction(num) {
  return num * 10;
}
```
#### filter 
it calls a true/false function on each item and creates a new array with only the items where the function values true.
```javascript
const ages = [32, 33, 16, 40];
const result = ages.filter(checkAdult);

function checkAdult(age) {
  return age >= 18;
}
```

### ✍️Topic 5 -> spread `...`
it let us take all the items in an array and spread them around.
- one common use of `...` is to concat two arrays in one new one.
```javascript
let arr1 = [1,2,3];
let arr2 = [3,4,5];
let arr3 = [...arr1, ...arr2];
```
equivalent to 
```javascript
let arr1 = [1,2,3];
let arr2 = [3,4,5];
let arr3 = arr1.concat(arr2);
```



## Challenges
- [challenge 1](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-multiple-conditional-ternary-operators)
```javascript
//my solution
function checkSign(num) {
  return num > 0? "positive": num===0? "zero": "negative";
}
```

## Challenges
- [challenge 2](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-the-map-method-to-extract-data-from-an-array)
```javascript
//my solution
const ratings = watchList.map(item => ({
  title: item["Title"],
  rating: item["imdbRating"]
}));
```

## Challenges
- [challenge 3](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-the-filter-method-to-extract-data-from-an-array)
```javascript
//my solution
const filteredList = watchList
  .filter(x => {
    // return true it will keep the item
    // return false it will reject the item
    return parseFloat(x.imdbRating) >= 8.0;
  })
  .map(s => {
    return {
      title: s.title,
      rating: s.imdbRating
    };
  });
```
## Problem
- [problem](https://www.codewars.com/kata/5865918c6b569962950002a1/train/javascript)
```javascript
//my solution
function strCount(str, letter){  
  let sum = 0;
  for (let i=0; i<str.length; i++) {
    if (str[i]==letter) {
      sum ++;
    }
  }
  return sum;
}
```




