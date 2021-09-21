# FUNCTIONAL PROGRAMMING

## What is functional programming ?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

## What is a pure function and how do we know if something is a pure function ?

So how do we know if a function is pure or not? Here is a very strict definition of purity:

* It returns the same result if given the same arguments (it is also referred as deterministic)

* It does not cause any observable side effects

*`It returns the same result if given the same arguments`*.

## What are the benefits of a pure function ?

The code’s definitely easier to test. We don’t need to mock anything.

## What is immutability ?

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

## What is Referential transparency ?

Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

*`pure functions + immutable data = referential transparency`*

## What is a module ?

Module in Node.js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node.js application.

## What does the word ‘require’ do ?

Node.js follows the CommonJS module system, and the builtin require function is the easiest way to include modules that exist in separate files. The basic functionality of require is that it reads a JavaScript file, executes the file, and then proceeds to return the exports object.

## How do we bring another module into the file the we are working in ?

To include functions defined in another file in Node.js, we need to import the module. we will use the require keyword at the top of the file.

## What do we have to do to make a module available ?

To access the module functions, we have to export the functions.