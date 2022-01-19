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

- `.then(func)` doesn't mean the function will be executed right away, instead it's just telling us func will be executed once the promise is fulfiled (a value is returned). i.e. It puts the function to the `onFulfilment` array of the promise

- There are 2 kinds of fasade functions, one only returns a web browser feature and another will

  1. call the web browser feature

  2. return an object (promise) that has a status (pending, resolved, rejected) and some placeholders immediately

     * value - a placeholder for what will be returned from web browser feature

     * onFulfilment - an array for functions to be executed after the value is returned

     * onRejection - an array which we can store functions using `.catch()` in

- For the second type of fasade functions, JavaScript provides another queue called `microtask queue` (a.k.a. job queue) to store the functions returned from web browser feature. Event loop moves functions in this microtask queue to callback stack before it moves the functions in callback queue. i.e. microtask queue is for fasade functions that return promises

- Asynchronous JavaScript is the backbone of the modern web - letting us build fast "non-blocking" applications. Promises, Web APIs, the callback & microtask queues and event loop allow us to defer our actions until the work (an API request, time etc) is completed and continue running our code line by line in the meanwhile

### Iterators

### Generators
