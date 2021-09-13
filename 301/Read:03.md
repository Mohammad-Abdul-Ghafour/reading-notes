# Passing Functions as Props

## Map Methode :
**`Map`** method is a loop that iterate over an array and modify its elements using a callback function.

Instead of manually iterating over the array using a loop, you can simply use the built-in **`.map()`** method.

**`.map()`** method returns a new array that has the same length of the iterated array and each element being the result of the callback function.

### How to use loop to loop through array and display each value in JSX, how do I do that in React ?

There are many ways to do so, but I'm going to explain one of them.
let say we have array called arr:

```
class Main extends React.Component {
    render() {
        return (
            <div>
                {arr.map(element => {
            return (element);
        });}
            </div>
        );


    }
}
export default Main;
```

Here the map method returns the element value in each iteration to the div, so we will end having all value inside the div.

## List :
Lists are used to display data in an ordered format and mainly used to display menus on websites. In React, Lists can be created in a similar way as we create lists in JavaScript, but in React there is one additional thing we should add which is **`key`**.

In React each list should have unique **`key`**, *`keys`* help React identify which items have changed, are added, or are removed. *`Keys`* should be given to the elements inside the array to give the elements a stable identity.

## Spread Operator :

![Spread Operator](https://livecodestream.dev/post/how-to-use-the-spread-operator-in-javascript/featured_hu552373e3dd9cfa7192fd6d6eeac47a64_53660_680x0_resize_q75_box.jpg)

The **`spread operator`** is a new addition to the set of operators in JavaScript ES6. It takes in an iterable and expands it into individual elements. The spread operator is commonly used to make shallow copies of JS objects. Using this operator makes the code concise and enhances its readability.

The **`spread operator`** syntax: three dots *`…`* .

The *`…`* spread operator is useful for many different routine tasks in JavaScript, including the following :
* **`Copying an array`** :
    * Using the *`…`* spread operator is a convenient way to copy an array or combine arrays, and it can even add new items.
* **`Concatenating or combining arrays`** :
    * As seen in the last example, the spread operator can quickly combine two arrays, an operation known as array concatenation.
    
For Example :
```
const myArray = [`1`,`2`,`3`]
const yourArray = [`4`,`5`,`6`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // [1,2,3,4,5,6]
```
* **`Adding an item to a list`** :
    * Asnoted in the last example, the spread operator can add an item to an another array with a natural, easy-to-understand syntax:

For Example :
```
cconst myArray = ['3','4','5']
const yourArray = ['1', '2', ...myArray]
console.log(yourArray) //  Array(5) [ "1", "2", "3", "4", "5" ]
```

* **`Combining objects`** :
    * The spread syntax is useful for combining the properties and methods on objects into a new object.
    
```
const objectOne = {hello: "hello"}
const objectTwo = {world: "world"}
const objectThree = {...objectOne, ...objectTwo, Welcome: "Welcome"}
console.log(objectThree) // Object { hello: "hello", world: "world", Welcome: "Welcome" }
```

## Passing Function Component :
How to Pass Functions Between Components?
The first thing we should write the function in the parent component.

The increment function change the state from false to true.

How can you pass a method from a parent component into a child component ?
We pass a method from a parent to child using props.

How does the child component invoke a method that was passed to it from a parent component ?
using **`this.props.propsname`**.
