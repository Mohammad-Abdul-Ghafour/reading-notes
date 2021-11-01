# FileIO & Exceptions
## Read & Write Files in Python :

![Read & Write](https://data-flair.training/blogs/wp-content/uploads/sites/2/2018/02/Python-Files-IO-01.jpg)

First before we get into *`Read`* & *`Write`* What is a *`File`*?

* **`Files`** are composed of three main parts:
   1. **`Header`** : metadata about the contents of the file.
   2. **`Data`** : contents of the file as written by the creator or editor.
   3. **`End of file`** (*`EOF`*) : special character that indicates the end of the file.

And to access a file you need it's path.

* **`Paths`** is a string that represents the location of a file and it's contain three main parts :
   1. **`Folder Path`** : the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows).
   2. **`File Name`** : the actual name of the file.
   3. **`Extension`** : the end of the file path pre-pended with a period (.) used to indicate the file type.

Here’s a quick example:

```
/
│
├── path/
|   │
│   ├── to/
│   │   └── me.gif
│   │
│   └── My_text.txt
|
└── new.csv
```

### Opening and Closing a File in Python:
When you want to work with a file, the first thing to do is to open it.

This is done by invoking the **`open()`** which take a single required argument that is the path to the file.**`open()`** has a single return, the file object.

```
file = open('My_text.txt')
```

### Reading and Writing Opened Files:
Once you’ve opened up a file, you’ll can to read or write to the file.

Lets start with **`READ`** :

1. **`READ`** :
There are multiple methods that can be called on:
   1. **`.read()`** :This reads the entire file.
   2. **`.readlines()`** : This reads the remaining lines from the file object and returns them as a list.

```
>>> with open('My_text.txt') as reader:
>>>     print(reader.read())
```

```
>>> with open('My_text.txt') as reader:
>>>     print(reader.readline(5))
```

2. **`WRITE`** :
There are multiple methods that are useful for writing to a file:
   1. **`.write(string)`** : This writes the string to the file.
   2. **`.writelines(seq)`** : This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s).

```
>>> with open('My_text.txt') as writer:
>>>     writer.write(breed)
```

## Exceptions in Python :

![Exceptions in Python](https://www.freecodecamp.org/news/content/images/2019/12/Exception-Handling-in-Python.png)

What is **`Exceptions`** ?

In Python, an error can be a syntax or an exception errors.

So what is syntax and exception error ?

* **`Syntax Errors`** : occur when the parser detects an *`incorrect statement`*

```
>>> print( 0 / 0 ))
  File "<stdin>", line 1
    print( 0 / 0 ))
                  ^
SyntaxError: invalid syntax
```

* **`Exception Errors`** : This type of error occurs whenever *`syntactically`* correct Python code results in an error.

```
>>> print( 0 / 0)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ZeroDivisionError: integer division or modulo by zero>>> print( 0 / 0)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ZeroDivisionError: integer division or modulo by zero
```
### Raising an Exception :

![Raising an Exception](https://static.javatpoint.com/python/images/python-exception-handling.png)

We can use raise to throw an exception if a condition occurs.

If you want to throw an error when a certain condition occurs using raise, you could go about it like this:

```
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
```

