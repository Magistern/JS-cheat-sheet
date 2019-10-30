# JS Cheat-sheet
Helpful snippets and common solutions to issues found out during the lab sessions.

## From Lab01
### Addition, Substraction, Multiplication, and Division of variables
- The **`prompt();`** method always **returns** a **string value**, thus, for some mathematical operations this string value **has to be converted to number value**.

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
Notice that the result of `console.log(sum)` is not 210, but "20010". This happens because, when `sum` is declared, the variable `input` is a string and 10 is a number. At this point, JavaScript is confused, since it does not know if what you want to do is:
1.  To join the values together (&quot;200&quot; + 10 = &quot;20010&quot;), or
1.  To add the values up (&quot;200&quot; + 10 = 210).

Because of this confusion, String values plus Number values will always result in a string with all the values &quot;glued&quot; together.

#### Solution:
You can directly declare the `input` variable as a number, by using any of the following alternatives:
```js
var input = Number(prompt("Enter any number:")); // used for integers and fractional numbers
var input = +prompt("Enter any number:"); // used for integers and fractional numbers
var input = parseInt("Enter any number:"); // used for integers only
var input = parseFloat("Enter any number:"); // used for integers and fractional numbers

var sum = input + 10;
console.log(sum); // 210
```
You can also perform the conversion after the value has been received from `prompt();`.
- Example 01
```js
// Just as above, this technique will permanently set `input` as a number.
var input = prompt("Enter any number:");
input = Number(input);
input = +input;
input = parseInt(input);
input = parseFloat(int);

var sum = input + 10;
console.log(sum); // 210
```
- Example 02
```js
// In this case, `input` will remain a string, it is just consider a number for this particular operation.
var input = prompt("Enter any number:");

var sum = Number(input) + 10;
var sum = +input + 10;
var sum = parseInt(input) + 10;
var sum = floatInt(input) + 10;
console.log(sum); // 210
console.log(typeof input); // string
```

#### Want to know more?
 MDN references: [prompt()](https://developer.mozilla.org/en-US/docs/Web/API/Window/prompt), [Number()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number), [+](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Unary_plus_%28%29), [parseInt()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt), [parseFloat()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseFloat), [typeof](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof).
