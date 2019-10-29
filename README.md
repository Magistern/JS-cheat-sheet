# JS cheat-sheet
Helpful snippets for labs

## Lab 1

| Troubleshooting                   | Things to Remember                                           | Comment                                                      |
| --------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `var age = prompt(“Your age is:”);` | `prompt()` always returns a string value, <br />if you need  to make operations <br />(sum, divide, etc.), the value needs to be converted to  number value. | To convert string value to a number, use any of the  following solutions: <br />var age = Number(  prompt(“Your age is:”) );<br />var age = +prompt(“Your  age is:”); <br />var age = parseInt(  prompt(“Your age is:”) );<br />var age = parseFloat(  prompt(“Your age is:”) ); |

 MDN reference s: [Number()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number), [+](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Unary_plus_()), [parseInt()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt), [parseFloat()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseFloat),

