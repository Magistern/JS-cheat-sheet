# JS Cheat-sheet
Helpful snippets and summary from the labs.

## From Lab01
### Addition, Substraction, Multiplication, and Division of variables
- The `prompt();` method always return a string value, thus, for some mathematical operations, this **string value has to be converted to number value**.

```js
var input       = prompt("Enter any number:"); // 200
var sum         = input+10;
var substract   = input-10;
var multiply    = input*10;
var divide      = input/10;

console.log(sum); // "20010"
console.log(substract); // 190
console.log(multiply); // 2000
console.log(divide); // 20
```
Notice that the result of `console.log(sum)` is not 210, but "20010". This happens because, when `sum` is declared, the variable `input` is a string and 10 is a number. At this point, JavaScript is confused, because it does not know if what you want to do is:
1.  To join the values together (&quot;200&quot; + 10 = &quot;20010&quot;), or
1.  To add the values up (&quot;200&quot; + 10 = 210).

Because of this confusion, String values plus Number values will always result in a string with all the values &quot;glued&quot; together.

#### Solution:
To fix this issue, you can use any of the following solutions that fits your code:
```js
var input = Number(prompt("Enter any number:")); // used for integers and fractional numbers
var input = +prompt("Enter any number:"); // used for integers and fractional numbers
var input = parseInt("Enter any number:"); // used for integers only
var input = parseFloat("Enter any number:"); // used for integers and fractional numbers

var sum   = input+10;
console.log(sum); // 210
```

##### Want to know more?
 MDN references: [Number()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number), [+](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Unary_plus_%28%29), [parseInt()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt), [parseFloat()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseFloat).
