# JavaScript

* [this](https://www.freecodecamp.org/news/the-complete-guide-to-this-in-javascript/) - The `this` reference inside functions can ****be bound to**** different objects depending on where the function is being called.
* JavaScript is **single threaded (one command executing at a time) and has a synchronous** execution model (each line is executed in order the code appears)

### Asynchronous

We use web browser features to achieve asynchronous

- **setTimeout** (a fasade function for web browser feature) returns a web browser feature called Timer. When the time is up, web browser will add the function to callback queue (a.k.a. task queue)
- **Event Loop: Functions in callback queue are allowed to go back to JavaScript when the call stack is empty and all the global code is finished running**

[Event Loop](./images/event-loop.jpeg)

* Callback queue is a JavaScript engine feature

### Promises

### Iterators

### Generators
