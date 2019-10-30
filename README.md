# JS Cheat-sheet
Helpful snippets and summary from the labs.

## From Lab01
### Addition, Substraction, Multiplication, and Division of variables
- The `prompt();` method always return a string value, thus, for some mathematical operations, this **string value has to be converted to number value**.

```js
1. var input       = prompt("Enter any number:"); // 200
1. var sum         = input+10;
1. var substract   = input-10;
1. var multiply    = input*10;
1. var divide      = input/10;
1.
1. console.log(sum); // "20010"
1. console.log(substract); // 190
1. console.log(multiply); // 2000
1. console.log(divide); // 20
```
Notice that the result of the sum on line 7 is not 210 but 20010. This happens because the variable `input` is a string, and JavaScript does not really know if what you want to do is:
1.  Joining the values together (&quot;200&quot;+10 =&quot;20010&quot;), or
1.  Adding the values (&quot;200&quot;+10=210).

String values plus number values, will give as a result a string with both values &quot;glued&quot; together.

#### Solution:
To fix this issue you can use the solution that fits your code.
```js
var input = Number(prompt("Enter any number:")); // Any number (1, 1.5)
var input = +prompt("Enter any number:"); // Any number (1, 1.5)
var input = parseInt("Enter any number:"); // Only for integers (1, 2, 3)
var input = parseFloat("Enter any number:"); // For fractional numbers (1.1, 3.75)
```

##### Want to know more?
 MDN references: [Number()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number), [+](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Unary_plus_%28%29), [parseInt()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt), [parseFloat()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseFloat).
