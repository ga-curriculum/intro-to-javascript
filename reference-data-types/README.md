# Intro to JavaScript - Reference Data Types

The seven data types we've looked at thus far are classified as **primitive/value** data types because they hold only a **single value**.

Most programming languages also have **complex/reference** data types designed to hold more complex data structures.

JavaScript only has one **reference** type - the **object**. That being said, there are several types of objects in JavaScript:

  - Array
  - Object
  - Function
  - RegEx
  - Date

## Objects

Objects are collections of zero or more key:value pairs known as properties.

We will learn more about *objects* in a later lesson.

For now, let's just verify what `typeof` returns:

```js
// We'll try an object
let myObject = {course: 'SEI', cohort: 4} // Object
console.log(typeof myObject)

// An array
let myArray = [] 
console.log(typeof myArray)

// And a Regular Expression
let myRegEx = /./ 
console.log(typeof myRegEx)
```

Although *functions* are also considered objects (*callable objects* to be exact), the `typeof` operator returns a more helpful data type:

```js
let myFunction = function(){}
console.log(typeof myFunction)
```

> ❓ If a variable is not a string, number, boolean, null, undefined, bigint, or a symbol, it must be an _________.