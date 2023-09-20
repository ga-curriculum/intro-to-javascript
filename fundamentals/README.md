# Intro to JavaScript - Fundamentals

## Making Comments

In JavaScript and many other programming languages, we can make our more readable and maintainable for ourselves and others by writing **comments**. Comments are pieces of tiext that are ignored by the JavaScript interpreter.

There are a number of reasons why comments in JavaScript are important and useful to us, including:
  - They help us understand our code when we come back to it later. 
  
  - They help others understand our code (this is especially important when working on team projects).
  
  - They help document our code's functionality, which can aid in troubleshooting and debugging. 

### How to write comments in JavaScript

There are two types of comments in JavaScript: **single-line** and **multi-line**. 

#### Single-line comments

Single-line comments start with two forward slashes `//` and continue to the end of the line. Everything on that line after the forward slashes is ignored by the JS interpreter.

```js
// This is a single-line comment.
```

You can either write single-line comments on their own line, or on the same line as code (but this can get a bit messy). The forward slashes will ignore the code written before them.

```js
console.log('Comments are great') // I only ignore words written after me!
```

#### Multi-line comments 

Multi-line comments in JavaScript are opened with a forward slash and an asterisk `/*` and closed by an asterisk and a forward slash `*/`. Anything written between the start and end tags is ignored by the JS interpreter.

```js
/* 
This is a multi-line comment.
It can span multiple lines. 
*/
```

You can use comments to document things like:
  - The purpose of your code

  - The input and output of your functions

  - Any known issues with your code

  - Why a decision was made in a code block, or to provide context

## Printing to the console

The console is a tool that allows us to interact with our JavaScript code. We use it to print an output, run commands, and debug our code!

To print to the console in JavaScript, we can use the `console.log()` function. This function takes any number of arguments and prints them to the console. 

```js
console.log('Hello, world!') // This prints 'Hello, world!' to the console
```

Printing to the console, or console logging, is one of the most powerful tools we have at our disposal for understanding and debugging our code. Console logging early and often is one of the best ways to learn JavaScript. 