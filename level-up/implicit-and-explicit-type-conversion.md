# Implicit and Explicit Type Conversion

## Type Conversion

JavaScript is very relaxed when it comes to data types. Contrary to non-dynamic languages, a variable can change its type.

```js
let m = 15 // I'm a number
m = 'hey' // Now I'm a string!
```

## Beware of implicit conversion

**Implicit type conversion** is the process of automatically converting one data type to another. JavaScript performs implicit type conversion in a variety of situations, such as when you perform arithmetic operations on values of different types.

JavaScript is friendly and tries to help us whenever it can. However, we all know that sometimes it's better to be left alone.

**Try adding a string to a number. What did JS do?**

Now try comparing a number and a string containing the same digits using the equality (`==`) comparison operator:

```js
13 == "13" // returns true!
```

This is why, unless there's a reason not to do so, we use the *strict equality operator* (`===`) as it will not perform type conversion.


## Explicit type conversion

**Explicit type conversion** is the process of manually converting one data type to another. You can use the following methods to perform explicit type conversion:

To convert into strings: 

  - using the `toString()` method

    ```js
    let n = 123.456;
    let s1 = n.toString(); // "123.456"
    ```
  
  - using the `String()` method

    ```js
    let n = 123.456;
    let s1 = String(n); // "123.456"
    ```

  - using the `toFixed()` method

    ```js
    let n = 123.456;
    let s1 = n.toFixed(2); // "123.46"
    ```
  Note that we need to specify the number of decimals we want inside of the `()`'s.

To convert into numbers:

  - using the `parseInt()` method 

    ```js
    let s = "1234.567";
    let n1 = parseInt(s); // 1234
    ```
    `parseInt()` rounds down to the nearest whole number. 

  - using the `parseFloat()` method

    ```js
    let s = "1234.567";
    let n = parseFloat(s); // 1234.567
    ```

  - using the `Number()` method

    ```js
    let s = "1234.567";
    let n = Number(n); // 1234.567
    ```

## When to use implicit and explicit type conversion

Implicit type conversion can be convenient, but it can also lead to unexpected results. It's important to be aware of the situations in which JavaScript will perform implicit type conversion.

In general, it's best to use explicit type conversion when we need to be sure that a value is of a certain type. For example, if we're writing a function that expects a number value as a parameter, we should use the `Number()` function to convert the value to a number before using it in the function.


