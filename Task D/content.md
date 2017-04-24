# Functions

With functions, you can give a name to a whole block of code, allowing you to reference it from anywhere in your program. JavaScript has built-in functions for several predefined operations. Here are three some functions.

 ```
 alert("message")
 confirm("message")
 prompt("message")
 ```

### Function Example

* Open a html file and View the Source
* Put the cursor after " // add code here " and enter:

```
var userName
var willDoSurvey
userName = prompt("Enter your name", "")
alert("Thank you, " + userName)
```

#### Save the changes and Refresh the page

### User-Defined Functions

With user-defined functions, you can name a block of code and call it when you need it. You define a function in the HEAD section of a web page. It is defined with the function keyword, followed by the function name and any arguments.

```
function functionName(argument)
{
statements
}
```