# Topic II
## Classes and Objects :
1. **`Classes`** : Provide a means of bundling data and functionality together. It holds it's own data members and member functions, which can be accessed and used by creating an instance of that class.*` A class is like a blueprint for an object`*.

Some points on Python class:

* Classes are created by keyword class.
* Attributes are the variables that belong to a class.
* Attributes are always public and can be accessed using the dot (.) operator.

2. **`Object`** : is an instance of a Class. A class is like a blueprint while an instance is a copy of the class with actual values.

An object consists of : 

* **`State`** : It is represented by the attributes of an object. It also reflects the properties of an object.
* **`Behavior`** : It is represented by the methods of an object. It also reflects the response of an object to other objects.
* **`Identity`** : It gives a unique name to an object and enables one object to interact with other objects.

An example :

```
class Person:

    def __init__(self, name):
        self.name = name

    def say_hi(self):
        print('Hello, my name is', self.name)
 
p = Person('Nikhil')
p.say_hi()
```

1. **`self`** :
   * Class methods must have an extra first parameter in the method definition. We do not give a value for this parameter when we call the method, Python provides it.
   * If we have a method that takes no arguments, then we still have to have one argument.
   * This is similar to this pointer in C++ and this reference in Java.
2. **`__init__ method`** : The __init__ method is similar to constructors in C++ and Java. Constructors are used to initializing the object’s state.

![Classes and Objects](https://learnscripting.org/wp-content/uploads/2019/09/Class-Concept.png)

## Thinking Recursively :
Problems can often seem big and scary. But we can break them down into smaller problems enough to solve. This is the essence of thinking recursively.

A recursive function has to fulfil an important condition to be used in a program *`it has to terminate`*. A recursive function terminates, if with every recursive call the solution of the problem is downsized and moves towards a base case.

A simple example on factorial:

```
4! = 4 * 3!
3! = 3 * 2!
2! = 2 * 1
```

Replacing the calculated values gives us the following expression

```
4! = 4 * 3 * 2 * 1
```

In other words, recursion in computer science is a method where the solution to a problem is based on solving smaller instances of the same problem.

```
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)
print(factorial(5))

Output : 120
```
![Thinking Recursively](https://files.realpython.com/media/Thinking-Recursively-in-Python_Watermarked.1825397c00ea.jpg)

## Fixtures and Coverage :
1. **`Fixtures`** : They provide a fixed baseline so that tests execute reliably and produce consistent, repeatable, results.

In pytest, you define fixtures using a combination of the *`pytest.fixture`* :

```
def reverse_lines(f):
   return [one_line.rstrip()[::-1] + '\n'
           for one_line in f]
```

Here's how that looks in pytest:

```
@pytest.fixture
def simple_file():
   return StringIO('\n'.join(['abc', 'def', 'ghi', 'jkl']))
```

![Fixtures](https://files.realpython.com/media/Intermediate-Advanced-PyTest-Features_Watermarked.2d8ace6b71be.jpg)

2. **`Coverage`** : is a tool for measuring code coverage of Python programs. It monitors your program, noting which parts of the code have been executed, then analyzes the source to identify code that could have been executed but was not.

For example, let's assume you have a very strange function, only_odd_mul, which multiplies only odd numbers:

```
def only_odd_mul(x, y):
   if x%2 and y%2:
       return x * y
   else:
       raise NoEvenNumbersHereException(f'{x} and/or {y}
 ↪not odd')
```

Here's a test you can run on it:

```
def test_odd_numbers():
   assert only_odd_mul(3, 5) == 15
```

![Coverage](https://lh3.googleusercontent.com/proxy/eELMsGknE-x5MhWy2fYIp3kgLbqdxVusUudselm8liu4nN98XmOOFjbFr3TeA7Is0ng4TDkGmlDkj_5SpChbw9W36gglvDlPylwnhMpmFA-ljkNzKKJHchs)