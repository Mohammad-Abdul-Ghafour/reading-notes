# Problem Domain, Objects, and the DOM
## Problem Domain:
In this class we will learn about problem domain.

Understanding the problem domain is the **hardest** part of programming.
### What is problem domain ?
The problem domain basically explains that you cannot fix if you does not understand what needs fixing. To be efficient and effective software developers must first undertand the problem thu and thru before starting to write code.

If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:
* **Make the problem domain easier**
    * You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.
* **Get better at understanding the problem domain**
    * It is easy to fall into the trap of thinking you understand enough of the problem to get started coding it.

## Objects :
### What is Objects in JS :
An object is a collection of properties, and a property is an association between a name (or key) and a value. As follows :
```
let objectName = {
    key: value
}
```
### What is the benefit of Objects ?
Let's say you want to enter personal data first name, last name, age, and ID number and more data you need a lot of variables. So in object we can avoid declaring lots of variables by declaring only one and assign all values you need to this variable.

EXP :
```
let personalData = {
    firstName: "Mohammad";
    lastName: "Abdul Ghafour";
    age: 27;
}
```
## Document Object Model (DOM) :
### What is DOM:
It represents the page so that programs can change the document structure, style, and content. 

In other words DOM is to manipulate HTML documents.
### DOM Tree :
The DOM represents HTML as a tree structure of tags. Here’s how it looks:
![DOM Tree](https://www.researchgate.net/profile/Jian-Chang-8/publication/254002847/figure/fig1/AS:298235726974978@1448116346303/Example-of-DOM-Node-Tree.png)

Every tree node is an object.

According to the Document Object Model (DOM), every HTML tag is an object. Nested tags are “children” of the enclosing one. The text inside a tag is an object as well.

All these objects are accessible using JavaScript, and we can use them to modify the page.
### How to use DOM ?
There is lots of way to manipulate HTML. But the most common way to access an HTML element is to use the id of the element.

`getElementById` method used `id="demo"` to find the element.

EXP :
```
const element = document.getElementById("intro");
```
And as we said there is many ways to manipulate HTML like :
* *getElementsByTagName*
* *getElementsByClassName*
* *querySelectorAll*

And more ...
