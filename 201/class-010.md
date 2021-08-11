#  JS Debugging
## What is debugging :
Programming code might contain syntax errors, or logical errors.
Searching for (and fixing) errors in programming code is called code debugging.

## ORDER OF EXECUTION :

The order of execution means that some code cann't be executed before others.
In other words lets take a simple example :

```
function sum(a,b){
return a + b
}
sum(x,y);
let x = prompt("asd")
let y = prompt("asdqw")
```
Here we cann't invoke the function before we let the user enter the two numbers. So the code should be as follows :
```
function sum(a,b){
return a + b
}
let x = prompt("asd")
let y = prompt("asdqw")
sum(x,y);
```
So understanding the order of execution of your code is most umportant thing for the debugging.

## FINDING AND FIXING THE ERROR :
### Finding the error :
Finding the error has many way but for me I follow these steps :
1. Using the browser *console*.
    * The browser *console* is the best *tool* to start searching for your errors.

![browser console](https://developer-chrome-com.imgix.net/image/admin/lMl9U6EJBQDLBVYKbxX9.png?auto=format)

2. If the error didn't shown in the console or you don't understand the error use **`console.log()`** statement.

    * **`console.log()`** also very helpful to find your error.
![console](https://i.stack.imgur.com/bRyBl.png)

And there is many way to find where is your error.
### Fixing the error :
Now that you know what an error is and how to find them, there are two things you can do with the errors.
* Fixing the error :
    * You will need to debug the code, track down the source of the error, and fix it.
* Handle errors :
    * You can handle errors using **`try`**, **`catch`**, **`throw`**.
