# ⭐️Day Two (JUL 4 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> Valuse and Data Types
information (data) in javaScript can be of diffrent types:
- strings: it can be between double quotes `" "`, single quotes `' '` or backticks.
- numbers: it can be positive or negative integers, flaoting numbers and also infinity.
- boolean: true or false.
- undefined: accidental nothing & its type is undefined.
- null: deliberate nothing & its type is object.
- others --we will learn about it later--

> - `typeof` tells us the type of value ex. `typeof true  //boolean`
> - 4 != "4"
> - data types in javaScript can be primitive (ex. string, number) or object (ex. document)

### ✍️Topic 2 -> strings 
strings made of small units called characters
> in string, characters are in specific order, each gets a number, starting at 0
#### string methods 
- .length: return a number represent how many characters in the string
- .indexOf(): tell us what is the index of a specific character or what index does another string begin
> if there are more than one character in the string, it will return the position of the first appearence
> if the character or substring is not exist, it will return -1
- .includes():check whether or not a string includes another string, it returns true/ false
- .startsWith(): ask if string begins with some other string, it returns true/ false
- and others

### ✍️Topic 3 -> operators
- `+` to add two numbers or concatinate two strings
- `-` to subtract two numbers
- `*` to multiply two numbers
- `/` to divide one number by another

### ✍️Topic 4 -> comparison operaters
`>` `<` `>=` `<=` `==` `!=` `===` `!==`
> `===` (strict equals) is differ from `==` (loosey-goosey) in that `===` compare valuse and datatypes wgile `==` only compare values

## Challenges
- [challenge 1](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-bracket-notation-to-find-the-nth-to-last-character-in-a-string)
```javascript
// my solution
// Setup
const lastName = "Lovelace";

// Only change code below this line
const secondToLastLetterOfLastName = lastName[lastName.length-2]; // Change this line
```


## Problem
- [problem](https://www.codewars.com/kata/56a1c074f87bc2201200002e/train/javascript)
```javascript
// my solution
function smaller(nums) {
    const res = [];
    let sum = 0;
    for (let i=0; i<nums.length; i++) {
        for (let j=i; j<nums.length; j++) {
            if (nums[j]<nums[i]) {
                sum ++;
            }
        }
        res.push(sum);
        sum = 0;
    }
    return res
}
```
