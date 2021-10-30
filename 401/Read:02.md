# Testing and Modules
## In Tests We Trust - TDD with Python :
What is Unit tests and TDD :

* **`Unit tests`** : are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.
* **`TDD`** (*`Test-Driven Development`*) : is a strategy to think in which test cases are developed to specify and validate what the code will do.

Other thing to care about is the structure. A convention widely used is the **`AAA`**:*` Arrange`*, *`Act`* and *`Assert`*.
* **`Arrange`** : you need to organize the data needed to execute that piece of code (input).
* **`Act`** : here you will execute the code being tested (exercise the behaviour).
* **`Assert`** : after executing the code, you will check if the result (output) is the same as you were expecting.

### TDD Cycle :
**`TDD Cycle`** is an important thing about TDD, the cycle is made by three steps :
1. Write a unit test and make it fail.
2.  Write the feature and make the test pass.
3. Refactor the code.

![TDD Cycle](https://www.impactqa.com/wp-content/uploads/2018/11/tdd.jpg)

## If name equals main :
What does the if **`__name__`** == “**`__main__`**”: do?

![If Name = Main](https://codefather.tech/wp-content/uploads/2021/04/if-name-main-in-python-840x480.png?ezimgfmt=ng%3Awebp%2Fngcb10%2Frs%3Adevice%2Frscb10-2)

In simple words the code that is inside the ( if **`__name__`** == “**`__main__`**”: ) it will only run when the model itself executed directly.

And if the model imporded somewhere else it won't executed.

For example :

```
print ("Always executed")
 
if __name__ == "__main__":
    print ("Executed when invoked directly")
else:
    print ("Executed when imported")
```

In this code the first **`print`** will always executed but the second one won't be executed unless we are inside the same model or it will execute the third **`print`**.

## Recursion :
The process in which a function calls itself directly or indirectly is called **`Recursion`**.

For example :
Let us consider a problem that a programmer have to determine the sum of first n natural numbers, there are several ways of doing that but the simplest approach is simply add the numbers starting from 1 to n. So the function simply looks like,

```
approach(1) – Simply adding one by one

f(n) = 1 + 2 + 3 +……..+ n
```

but there is another mathematical approach of representing this,

```
approach(2) – Recursive adding 

f(n) = 1                  n=1

f(n) = n + f(n-1)    n>1
```

There is a simple difference between the approach (1) and approach(2) and that is in approach(2) the function “ f( ) ” itself is being called inside the function, so this phenomenon is named as **`Recursion`** and the function containing **`Recursion`** is called **`Recursive`** function.

How a particular problem is solved using recursion?

The idea is to represent a problem in terms of one or more smaller problems, and add one or more base conditions that stop the recursion. For example, we compute factorial n if we know factorial of (n-1). The base case for factorial would be n = 0. We return 1 when n = 0.

What is the difference between direct and indirect recursion?

A function fun is called direct recursive if it calls the same function fun. A function fun is called indirect recursive if it calls another function say fun_new and fun_new calls fun directly or indirectly.

An example of direct **`Recursion`** :

```
void directRecFun()
{
    // Some code....

    directRecFun();

    // Some code...
}
```

An example of indirect **`Recursion`** :

```
void indirectRecFun1()
{
    // Some code...

    indirectRecFun2();

    // Some code...
}
void indirectRecFun2()
{
    // Some code...

    indirectRecFun1();

    // Some code...
}
```