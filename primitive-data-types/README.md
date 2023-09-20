# Intro to JavaScript - Primitive Data Types

JavaScript has seven primitive data types, five of which are **common**, and two of which are **uncommon**.

## Common primitive data types

Here are the common primitive data types in JavaScript:

  - Boolean
  - Null
  - Undefined
  - Number
  - String

### string
A **string** represents textual data with zero or more characters wrapped by single or double quotation marks such as `"John"` or `'Jane'`. A pair of quotes with nothing between them is still a **string** - an empty *string*.

```js
let myString = 'Hello World'
let myOtherString = "Hello World"
console.log(typeof myString)
```
Note that the `typeof` operator itself always returns a string describing the data type.


> ❓ Is let _save = '' a valid statement?


### number
A **number** represents a numeric value.

Unlike many other programming languages, there is no distinction between integer (`15`, `3`, etc.) and floating-point/decimal types (`17.24`, `3.1416`, etc.).

Internally, JS represents all numbers as floating-point values.

```js
let myNumber = 15
console.log(typeof myNumber)
```

> ❓ What will the following code print to the console?

```js
console.log(typeof 12.34)
```

### boolean
Whereas strings and numbers can have a virtually unlimited number of different values, the **boolean** data type only has two possible values: `true` and `false`.

### null
The null data type has only one value: `null`. null is the value of a variable that explicitly has no value. Thus, it represents a lack of value. However...

```js
console.log(typeof null) // "object" 
```
Fail! JS was written in 10 days by one dude, so there are bound to be some issues. 

Because of this behavior, the use of null is somewhat controversial in the JavaScript community.

### undefined
A variable that has not been assigned a value is of type `undefined`. For example:

```js
let cohort // cohort currently holds undefined
console.log(cohort)
```

In addition, a function by default returns `undefined` if a value was not explicitly returned using the `return` keyword.

Lastly, you will see `undefined` if you enter code directly into the browser’s console and it evaluates a statement that does not return a value.

```js
console.log(typeof undefined)
console.log('hello')
```


## You do 💪: Data type examples
**Strings**, **numbers**, and **booleans** are the most common data types used to "model" real-world data in applications.

For example, in a multiplayer gaming app, we would represent a player's Gamertag using a **string**.

Before moving on to review the other data types, let's brainstorm a couple of examples for each of the three common data types that would be used to represent information in that gaming app:

#### Gaming app data types
| Data Type | Example Data/Information |
| ------ |:----------:|
| **String** | gamerTag,           |
| **Number** |                     |
| **Boolean** |                    |

## Uncommon primitive data types

Here are the uncommon primitive data types in JavaScript:

  - Symbol
  - BigInt

### symbol
The *symbol* data type was added with ES2015 and is primarily used to create unique and less visible properties on objects.

Their use is rare in general JavaScript programming.

### BigInt
Added with ES2015, a `bigint` value can hold a massive integer value but it is not commonly needed or used - primarily because it is incompatible with the `number` type and none of the `Math` object's methods work with it.

```js
let ourBigInt = 15n
console.log(typeof ourBigInt)
```

> ❓ Do all variables have a data type?

