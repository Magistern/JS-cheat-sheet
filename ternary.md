# JS Cheat-sheet
Helpful snippets and common solutions to issues found out during the lab sessions.

## Ternary Operator
The conditional (ternary) operator is the only JavaScript operator that takes three operands:
1. A condition followed by a question mark (?), then
2. an expression to execute if the condition is truthy followed by a colon (:), and finally
3. the expression to execute if the condition is falsy. This operator is frequently used as a shortcut for the if statement.
### Syntax
```js
//   1         2       3
(condition) ? true : false;
```
### Common Use
This operator is frequently used as a shortcut for the if statement.
```js
// Example: print a «msg» if the result of the multiplication is the number 50.
var a = 10;
var b = 5;
var multiply = a*b;
var msg;

// With a common if statement
if(multiply == 50) {
    msg = "Yes, I am #50";
} else {
    msg = "No, I am not #50";
}
console.log(msg); // Yes, I am #50

// Using Ternary Operators
msg = (multiply == 50) ? "Yes, I am #50" : "No, I am not #50";
console.log(msg); // Yes, I am #50
```

### References
 MDN references: [Conditional (Ternary) Operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator).
