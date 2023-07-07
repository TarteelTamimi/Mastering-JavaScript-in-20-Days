# ⭐️Day Four (JUL 6 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> objects
- objects collect multiple values together to describe more complex data.
- to declare an object we use `{ }`, ex. `const obj = {name:"Tarteel, age:20}`
- objects let us point at releted values using properties in the object, ex. `obj.name  //obj['name']`
- we can assign a new property on an existing object, ex.`obj.city = 'hebron'`, so the objects in javaScript are mutable
> to make the object immutable, we use `Object.freeze(obj)`
> this: let us reference other properties on the object
- we can put arrays in object, and objects in array
```javascript
//example
const p1 = {
name: 'Tarteel',
age: '20',
sisters: ['Majd', 'Sara']
}

const p2 = {
name: 'Najah',
age: '23',
sisters: ['Raghad', 'Sara', 'Mayar', 'Hala', 'Loma']
}

const people = [p1, p2, p3, ...]
```


## Challenges
- [challenge 1](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/profile-lookup)
```javascript
// my solution
// Setup
const contacts = [
  {
    firstName: "Akira",
    lastName: "Laine",
    number: "0543236543",
    likes: ["Pizza", "Coding", "Brownie Points"],
  },
  {
    firstName: "Harry",
    lastName: "Potter",
    number: "0994372684",
    likes: ["Hogwarts", "Magic", "Hagrid"],
  },
  {
    firstName: "Sherlock",
    lastName: "Holmes",
    number: "0487345643",
    likes: ["Intriguing Cases", "Violin"],
  },
  {
    firstName: "Kristian",
    lastName: "Vos",
    number: "unknown",
    likes: ["JavaScript", "Gaming", "Foxes"],
  },
];

function lookUpProfile(name, prop) {
  // Only change code below this line
  for (let i = 0; i < contacts.length; i++) {
    if (contacts[i].firstName === name) {
      if (contacts[i].hasOwnProperty(prop)) {
        return contacts[i][prop];
      } else {
        return "No such property";
      }
    }
  }
  return "No such contact";
  // Only change code above this line
}

lookUpProfile("Akira", "likes");
```


## Problem
- [problem](https://www.codewars.com/kata/5875b200d520904a04000003/train/javascript)
```javascript
// my solution
function enough(cap, on, wait) {
    return (cap - on) >= wait ? 0 : wait - (cap - on);
}
```
