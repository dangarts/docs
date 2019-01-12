# Javascript

## Operator Precedence

- [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence)

## Variables and Data Types

- 5 primitive data types
    - String
    - Number
    - Boolean
    - Null
    - Undefined
- JS has dynamic typing which automatically detects the type of the variable

## Ternary Operator

Alternate way of if/else conditional statements

```
var age = 21;
age >= 18 ? console.log('drinks beer')` : console.log('drinks juice');
```

condition ? if condition is met : else run this statement

## Truthy vs Falsy values

The following renders falsy values

- undefined
- null
- 0
- ''
- NaN

## Array Methods

- `nameOfArray.push('john');` //adds john to end of array
- `nameOfArray.unshift('john');` //adds john to the beginning of array
- `nameOfArray.pop();` //removes the last array element
- `nameOfArray.shift();` //removes the beginning array element
- `nameOfArray.indexOf('john');` //returns the index position of the arument
   - if the element is not in the array, the value `-1` is returned.  This is used for conditional statments.

## Hoisting

- Hoisting works only with function declarations and not function expressions.
   - Function Declaration: `function example(){}`
   - Function Expression: `var example = function(){}`

# Scoping

- Variables defined in the root is accessible everywhere and within functions.
- Global Execution Context
   - Is seperate environment to that within functions
   - If for example `var age` was used twice in the root code and also within a function.  The `age` in the function is defined in the variable object of the **execution context object** of the function and the root variable is defined in the variable of the **global execution context** object.

- Each new function creates a scope
- **Lexical Scoping**: a function that is lexically within another function gets access to the scope of the outer function.

- Scope Chain: Global execution is limited to variable access when variables are used within functions and nested functions.

- Execution stack vs scope chain
   - execution stack is the order functions are called
   - scope chain is the order in which functions are written lexically.

- The `this` keyword
   - In a method, `this` refers to the owner object.
   - Alone, `this` refers to the global object.
   - In a function, `this` refers to the global object.

## method borrowing

- Instead of rewriting a similar method in an object, you can use method borrowing to be used in a separate object.
   - Ex. `joe.calcAge = mike.calcAge` where `calcAge` is a method within the `joe` object.  When the mike object was created, instead of reusing the calcAge method, we simply used the instance in the joe object by storing the method via `joe.calcAge = mike.calcAge`