# Python Scope

![Python Scope](https://files.realpython.com/media/Scope-in-Python---LEGB-Rule_Watermarked.e5f68e7a3642.jpg)

The concept of scope rules how variables and names are looked up in your code. It determines the visibility of a variable within the code.

The Python scope concept is generally presented using a rule known as the *`LEGB`* rule, *`LEGB`* stand for *`Local`*, *`Enclosing`*, *`Global`*, and *`Built-in`* scopes.

In programming, the *`scope`* of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on.

Most commonly, you’ll distinguish two general scopes:
* **`Global scope`** :
   * The names that you define in this scope are available to all your code.
* **`Local scope`** :
   * The names that you define in this scope are only available or visible to the code within the scope.

But we will focus on **`Global`** and **`Nonlocal`** statement.

Every **`variable`** in python is limited to a certain scope. The scope of a python is the module-scope. Consider the following:

```
myvariable = 5 
 # myvariable has module-level scope

def func():
    x = 3      
     # x has "local" or function level scope.
```

Objects with local scope die as soon as the function exits and can never be retrieved (unless you return them), but within a function, you can access variables in the module level scope :

```
myvariable = 5
def func():
    print(myvariable) 
     # prints 5

def func2():
    x = 3
    def func3():
        print(x)      
         # will print 3 because it picks it up from `func2`'s scope

    func3()
```

However, you can't use assignment on that reference and expect that it will be propagated to an outer scope:

```
myvariable = 5
def func():
    myvariable = 6    
     # creates a new "local" variable.  
     # Doesn't affect the global version
    print(myvariable) 
     # prints 6

func()
print(myvariable)     
 # prints 5
```

Now, we're finally to global. The global keyword is the way that you tell python that a particular variable in your function is defined at the global (module-level) scope.

```
myvariable = 5
def func():
    global myvariable
    myvariable = 6   
     # changes `myvariable` at the global scope
    print(myvariable)
     # prints 6

func()
print(myvariable) 
 # prints 6 now because we were able 
 # to modify the reference in the function
```

In other words, you can change the value of myvariable in the module-scope from within func if you use the global keyword.

As an aside, scopes can be nested arbitrarily deep:

```
def func1():
    x = 3
    def func2():
        print("x=",x,"func2")
        y = 4
        def func3():
            nonlocal x 
             # try it with nonlocal commented out as well.  See the difference.
            print("x=",x,"func3")
            print("y=",y,"func3")
            z = 5
            print("z=",z,"func3")
            x = 10

        func3()

    func2()
    print("x=",x,"func1")

func1()
```

Now in this case, none of the variables are declared at the global scope, and in python2, there is no (easy/clean) way to change the value of x in the scope of func1 from within func3. That's why the nonlocal keyword was introduced in python3.x . nonlocal is an extension of global that allows you to modify a variable that you picked up from another scope in whatever scope it was pulled from.