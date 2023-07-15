# ⭐️Day Eleven (JUL 13 2023)

## To-Do List for today
- [x] Watch 90-minutes of courses-Frontend Masters
- [ ] Solve Challenges-Freecodecamp
- [x] Solve one problem-Codewars
- [x] Summarize what I learned

## Topics
### ✍️Topic 1 -> Asynchronous javaScript
javaScript is:
1. single threaded (one command run at a time).
2. synchronously executed (each line is run in order the code appears).

we can delay a function using `setTimeOut()`.

#### web browser is:

**javaScript + browser features**

each browser feature has a lable in javaScript: 
- console --> console
- network request --> xhr / frecth
- HTML DOM --> document
- Timer --> setTimeOut

> xhr: is javaScrit way to speak to the inter net

#### callback functions
the problems: 
1. our response data is only available in callback functions.
2. maybe it feels a little odd to think of passing of function into another function only for it to run much later.
the benefit:
1. super explicit one we understand how it works under-the-hood.

```javascript
function printHello() {
  console.log('Hello');
}
srtTimeOut(printHello, 1000);
console.log('me first!')

// it will print 'me first' first, then Hello.
 ```

#### Event loop
In JavaScript, the event loop is a fundamental part of the language's concurrency model. It is responsible for managing the execution of asynchronous code and handling events. The event loop ensures that JavaScript remains single-threaded while still allowing non-blocking I/O operations and asynchronous behavior.

explanation of how the event loop works:

1. JavaScript code is executed in a single-threaded environment, meaning that it can only execute one piece of code at a time.

2. When an asynchronous operation, such as a network request or a timer, is encountered, JavaScript doesn't block the execution. Instead, it registers the asynchronous task and continues with the next instructions.

3. Once the asynchronous task is completed, it's placed in a queue called the "task queue" or "callback queue".

4. The event loop continuously checks if the call stack (the place where synchronous code is executed) is empty. If it's empty, it picks the next task from the task queue and moves it to the call stack for execution.

5. This process of moving tasks from the task queue to the call stack is repeated as long as there are tasks in the queue.

By using the event loop, JavaScript can handle multiple asynchronous operations without blocking the execution of other code. It allows for the efficient handling of events, timers, and callbacks in web browsers and other JavaScript environments.


### ✍️Topic 1 -> Promises
it is an ES6 solution for asunchronous programming in javaScript
- it is initiate backgroung web browser
- work and return a placeholder object (promise) immediately in javaScript

```javascript
function display (data) {
  console.log(data);
}

const futureData = fetch('URL');
futureData.then(display);
console.log('Me first');
```
#### `.then()`
`then()` method is used in combination with promises to handle asynchronous operations and process the results or errors returned by those operations. The `then()` method is part of the Promise API and is used to specify what should happen after a promise is fulfilled (resolved) with a value or rejected with an error.

The `then()` method takes two callback functions as arguments: one for the success case (called when the promise is fulfilled) and one for the failure case (called when the promise is rejected).

#### Microtask queue
The microtask queue is where microtasks are queued for execution. Microtasks are tasks that need to be executed asynchronously but have a higher priority than regular tasks in the event loop. They are typically used for handling promises and other asynchronous operations that need to be resolved as soon as possible.

👎Problems
- 99% of developers have no idea how they’re working under the hood
- Debugging becomes super-hard as a result
- Developers fail technical interviews

  
👍Benefits
- Cleaner readable style with pseudo-synchronous style code
- Nice error handling process


## Challenges
- [challenges](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week2-day3-tasks/tasks.md)
```javascript
//challenge 1

```
## Problem
- [problem](https://www.codewars.com/kata/57ee24e17b45eff6d6000164/train/javascript)
```javascript
//my solution
function catMouse(x){
  return x.length > 5?'Escaped!': 'Caught!';
}
```
