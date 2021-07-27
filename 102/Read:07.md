# FUNCTIONS IN JS
### What is Functions?
A function in JavaScript is a block of statements that performs a task or calculates a value it should take some input and return an output.

### Why we use Functions for?
The main reason to use Functions in **JS** to eliminate code complexity by enabling re-usability. A function is a block of 'reusable code' that is used several times in the JavaScript program where it is defined

### How to use Functions?
JavaScript a function allows you to define a block of code, give it a name and then execute it as many times as you want. A function can be defined using function keyword and can be executed using () operator. A function can include one or more parameters.

We have two ways to write Functions:

1. Function declarations

This way consists of the function keyword, followed by:
* The name of the function.
* A list of parameters to the function, enclosed in parentheses and separated by commas.
* The JavaScript statements that define the function, enclosed in curly brackets, {...}.

**For example**
```
function sum(num,num1) {
  return num * num1;
}
sum(num,num1);
```
The function `sum` takes two parameter, called num & num1. The statement `return` specifies the value returned by the function which is num multiplied by num1.

2. Function expressions

Function Expression  allows us to create an anonymous function which doesn’t have any function name which is the main difference between Function Expression and Function Declaration.

**For example**

```
var sum = function(num,num1) { return num * num1 }
var x = sum(num,num1);
```
### What the difference between Function Expression and Function Declaration?

Function declarations load before any code is executed while Function expressions load only when the interpreter reaches that line of code.

So **Function Expressions** can be used as an Immediately Invoked Function Expressions (IIFE).

