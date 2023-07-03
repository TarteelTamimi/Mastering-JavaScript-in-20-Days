# ⭐️Day One

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [x] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what we learn

## Topics
> ### Topic 1 -> Introdution to JavaScript
- JavaScript is a dynamic programming language used usually in websites, so we can call it "programming language of the web".
- Created in 1995 by Brendon Eich.
- Used to modify and interact with HTML.
- We can run it in:
1. Browser
2. Servers - Node.js
3. Imbedded devices
                  
> ### Topic 2 -> DOM (Document Object Model)
#### Finding elements in a web page 
- document.title ==> represent the title of the page.
- document.body.children ==> all elements inside the body.
- .length ==> how many things in (ex.class).
- .textContent ==> the text element inside the selected one.

#### Changing a web page
We use the equal operator `=` to assign a value to the elements in the page.
* ex. `document.title = "My Page"     //will change the title of the page to My Page`


> ### Topic 3 ->


## Examples
```javascript
<body>
    <header>
    <h1>Tic Tac Toe</h1>
    <h2>A game you know</h2>


    <div id="players">
        <p id="p1" class="player">Player <span id="p1-symbol">X</span>: <span id="p1-name">Anjana</span></p>
        <p id="p2" class="player">Player <span id="p2-symbol">O</span>: <span id="p2-name">Marc</span></p>
    </div>
    </header>

    <div id="board">
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
    </div>
</body>

document.getElementsByTagName("p")                        //will return all p elements which are p1 & p2
document.querySelectorAll(".square").length               //will return the number of elements that have the class square which are 9
document.querySelector("h2").textContent                  //will return the text inside the element h2 which is "A game you know"
document.getElementById('p2-name').textContent = "Majd"   //will change the second player name to Majd
document.getElementById('p2-name').append(" & Sara")      //will add sara to the sacond player
document.querySelector("header h2").append(" and love")   //will append "and love" to the second header  
```

## Notes
- Document: Speciel built-in object that represent the whole page.
- MDN(Mozilla Developer Network) -> for reference end documentation.
- Difficults in JavaScript👎Validation / naming things / errors.
- Changes in Browser console will not be saved.


## Challenges & My Solutions
1. [challenge 1](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/compound-assignment-with-augmented-multiplication)
```javascript
let a = 5;
let b = 12;
let c = 4.6;

// Only change code below this line
a *= 5;
b *= 3;
c *= 10;
```

2. [challenge 2](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/concatenating-strings-with-the-plus-equals-operator)
```javascript
let myStr = "";

myStr += "This is the first sentence. This is the second sentence.";
```

3. [challenge 3](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-bracket-notation-to-find-the-nth-to-last-character-in-a-string)
```javascript
// Setup
const lastName = "Lovelace";

// Only change code below this line
const secondToLastLetterOfLastName = lastName[lastName.length-2]; // Change this line
```



## Problem & My Solution
- [problem](https://www.codewars.com/kata/564e7fc20f0b53eb02000106/train/javascript)
```javascript
function consonantCount(str) {
    let sum = 0;
    str = str.toLowerCase();

    for (let i = 0; i < str.length; i++) {
        if (str[i]!='i' && str[i]!='o' && str[i]!='e' && str[i]!='a' && str[i]!='u' && str[i]>='a' && str[i]<='z') {
            sum++;
        }
    }
    return sum;
}
```


