# Intro to JavaScript - Variables

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will understand the basics of JavaScript variables, including naming convetions and the difference between `let` and `const`.

## Concepts

The purpose of a [*variable*](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#declarations) in programming is to hold or reference data. 

> 📚 A *variable* is a named container that is used to store and retrieve data that is used within a program.

To create a variable in JavaScript, we use the `let` or `const` keyword followed by the variable name (also known as an identifier). 

```js
let favSnack // the identifier is "favSnack"
```

We can also assign a value to a variable at the time we declare it by using the `=` (assignment) operator:

```js
let name = 'Tony Stark'
```

and change its value later:

```js
name = 'Pepper Potts' // note that we only declare a variable once
```

 Multiple variables can be defined in a single statement, separated by commas:

```js
let name = 'Wilma', age, town = 'Bedrock'
// above is equivalent to
let name = 'Wilma'
let age
let town = 'Bedrock' 
 ```

## Naming rules

In JavaScript, when naming variables, the convention is to name the identifiers using lowerCamelCase, e.g., `numActivePlayers`.

Identifiers in JS:
  - Are case-sensitive!
  - Cannot begin with a number
  - Can contain letters, digits, underscores, and dollar signs
  - Cannot contain spaces
  - Cannot be [reserved words or keywords](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#keywords)

> ❓ Is car-3 a valid variable identifier?

## `let` and `const`

The difference between `let` and `const` is that a `const` variable cannot be re-assigned to - you can assign data to it once, and that's it:

```js
let x = 25
x = 100 // no problem
const z = 25
z = 100 // Uncaught TypeError: Assignment to constant variable
```

As we'll learn later, objects (or an object sub-type like array, function, etc.) are a reference type.

Objects are reference types, meaning that when you assign an object to a variable, the variable doesn't store the object itself, but rather a reference to the object in memory. This is why you can modify an object assigned to a `const` variable, but you can't reassign the variable itself:

```js
const person = {name: 'Fred'}
person.age = 25 // no error
person = {name: 'Barney'} // Uncaught TypeError: Assignment to constant variable
```

