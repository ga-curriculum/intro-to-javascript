# Weakly vs. Strongly Typed Languages

*Weakly-typed* languages such as JavaScript allow implicit conversions between types, which can lead to interesting results. For example:

```js
const num = 7
const sentence = "A week is " + num + " days."
console.log(sentence) // "A week is 7 days"
```

From the above, we can see that JavaScript will happily automatically convert the number 7 into a string so that it can be concatenated with the rest of the sentence. That same code in a strongly-typed language would not function. For example, in Python:

```python
num = 7
sentence = "A week is " + num + " days." 
# Error! A string and an int cannot be concatinated!
```

To make this valid code, the `num` must be explicitly converted into a string before it can be concatenated with the other strings surrounding it:

```python
num = 7
sentence = "A week is " + str(num) + " days." 
# This works!
print(sentence) # "A week is 7 days"
```

> 🧠 There is a newer language called TypeScript you might hear about - this language is a superset of JS and adds both static and strong typing to JS. Many developers agree that these type-safety features make code less error-prone and is worth the extra effort to code.


> 📚 In a *weakly-typed* language, conversions between unrelated data types occurs implicitly. In a strongly-typed language, conversions between unrelated data types must be explicitly made.

