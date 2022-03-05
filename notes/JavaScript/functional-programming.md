# Functional Programming in JavaScript

## Resouces

* Frontend Master: The hard parts of Functional JavaScript

---

- Function is a way to prevent unwanted side effect

- Functional programming comes from
    - Tiny functions: save every single line (or a few lines) as its own function
    - No consequences except on that line
    - Recombine/compose: build up our application by using these small blocks of self-contained code

- When you execute a function, you create a new execution context comprising:
    1. the thread of execution (we will go through the code in the function line by line)
    2. a local memory (variable environment) where anything defined in the function stored
    
    When the function returns, the execution context gets deleted

## Higher-order functions

- In JavaScript, functions are called **first class objects**. They can be treated like other JavaScript objects

- Callback function: a function we pass in another function (A) as a parameter. In this case, the function A is a higher-order function

## Map & Reduce

## `reduce`, `filter` and chaining higher order functions

## Function composition & pure functions

## Closure

## Function decoration

## Partial application and currying
