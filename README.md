# JS cheat-sheet
Helpful snippets for labs

## Lab 1

| Troubleshooting                   | Things to Remember                                           | Comment                                                      |
| --------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `var age = prompt(“Your age is:”);` | `prompt()` always returns a string value, if you need  to make operations (sum, divide, etc.), the value needs to be converted to  number value. | To convert string value to a number, use any of the  following solutions: <br />var age = [Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)(  prompt(“Your age is:”) );<br />var age = [+](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Unary_plus_())prompt(“Your  age is:”); <br />var age = [parseInt](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt)(  prompt(“Your age is:”) );<br />var age = [parseFloat](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseFloat)(  prompt(“Your age is:”) ); |

 

