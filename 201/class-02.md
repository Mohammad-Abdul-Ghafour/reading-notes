# Basics of HTML, CSS & JS
In this reading we will dig a little bit deeper in HTML, CSS and JavaScript.

## HTML :
### As we said before html stands for hypertext ***MARKUP*** language, so what is ***MARKUP*** means?

The markup tells web browsers how to display a web page's words and images. Each individual markup code is referred to as an element (*Tags*).

there is two different types of elements (tags):
1. Structural element
    * This elements that gives information about the structure of a document. It may also be associated with a change in appearance, but the key is that it provides information about divisions, titles, sections, paragraphs, or other aspects of the structure of a document.

    ![Most used Structural element](https://d2uusema5elisf.cloudfront.net/courses/30-days-of-webdev/day-07/public/assets/table-3.png)

2. Semantic element
    * Semantics refers to the correct interpretation of the meaning of a word or sentence. To use a word semantically is to use it in a way that is properly aligned with the meaning of the word.

![Most used Semantic element](https://miro.medium.com/max/1400/1*JgEkEenQwTNL55fAsbkNgA.png)

## CSS :
As we said CSS stands for Cascading Style Sheets, CSS specify how the content of an element should appear.

So what the benefits of CSS?
* CSS saves a lot of work. It can control the layout of multiple web pages all at once.
### CSS Rules :
CSS works by associating styling rules with HTML elements. The CSS rules govern how the contents of specified elements should be displayed. A CSS rule contains two parts :
1. A selector
2. One or more declarations

The selector specifies which HTML elements the rule applies to. The declarations indicate how the elements referred to by the selector should be styled and each declaration is split into two parts: a property ***name*** and a property ***value***.

![Selector Table](https://i0.wp.com/donnasresources.com/wp-content/uploads/2019/02/CSSSelectorTable.png?resize=590%2C575&ssl=1)

### How Css Rules Cascade ?
The CSS cascade assigns a weight to each style rule. When several rules apply, the one with the greatest weight takes precedence. By default, rules in author style sheets have more weight than rules in user style sheets.

## JAVASCRIPT :
As we said JavaScript is a interpreted scripting or programming language that allows you to implement complex and dynamical features on web pages to make web pages dynamic and interactive.

    A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a Statement.

**Statement** are used in JavaScript to control its program flow. 

### Variables in JS :
Variable means anything that can vary. In JavaScript, a variable stores the data value that can be changed later on. Use the reserved keyword var to declare a variable in JavaScript.

We use `var` or `let` or `const` to define variables.

**Here are rules JavaScript has for naming variables :**
* Variable names cannot contain spaces.
* Variable names must begin with a letter, an underscore (_) or a dollar sign ($).
* Variable names can only contain letters, numbers, underscores, or dollar signs.
* Variable names are case-sensitive.
* Certain words may not be used as variable names, because they have other meanings within JavaScript.Check out this [Complete List Of The Reserved Words](https://www.dummies.com/web-design-development/javascript/javascript-for-kids-for-dummies-cheat-sheet/) .

### Data Types in JS:
In Javascript, there are five basic, or primitive, types of data. The five most basic types of data are `strings`, `numbers`, `booleans`, `undefined`, and `null`( there is more data types ). We refer to these as primitive data types. A single variable can only store a single type of data.

![Data Types in JS](https://www.creatingux.com/CIT230/media/images/datatypes.png)

An array is a special variable, which can hold more than one value at a time.

If you have a list of items ( a list of car names, for example ), storing the cars in single variables could look like this:

```
let car1 = "Saab";
let car2 = "Volvo";
let car3 = "BMW";
```

An array can hold many values under a single name, and you can access the values by referring to an index number.

```
const cars = ["Saab", "Volvo", "BMW"];
```
### Operators in JS :
An operator is capable of manipulating a certain value or operand. Operators are used to perform specific mathematical and logical computations on operands.

 In JavaScript operators are used for compare values, perform arithmetic operations etc. JavaScript has the following types of operators:

* Assignment operators
* Comparison operators
* Arithmetic operators
* Bitwise operators
* Logical operators
* String operators
* Conditional (ternary) operator
* Comma operator
* Unary operators
* Relational operators

And there i will leave for you a table with the most important operators:

![OPERATORS TABLE](https://i.pinimg.com/originals/13/09/cb/1309cb725dea3e859a873607dd298d00.png)
