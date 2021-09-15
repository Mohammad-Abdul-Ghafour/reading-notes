# Putting it all together

## Thinking in React :

One of the many great parts of React is how it makes you think about apps as you build them.

![Thinking in React](https://miro.medium.com/max/1400/1*4QE3nTlCOGaynx1aWy9kuQ.png)

We are going to break the building React app prosses to 5 steps :

1. Break The UI Into A Component Hierarchy
2. Build A Static Version in React
3. Identify The Minimal (but complete) Representation Of UI State
4. Identify Where Your State Should Live
5. Add Inverse Data Flow

### What is the single responsibility principle and how does it apply to components ?
**`The Single Responsibility Principle`** means that a component should only do one thing.

![The Single Responsibility Principle](https://www.logiqlabs.com/wp-content/uploads/2021/04/SRP.png)

For Example : 

The *`header`* in the app should have it's own *`component`*  and the *`footer`* also it's own and so on.

### What does it mean to build a ‘static’ version of your application ?
**`Static app`** means that this version of the application has no interactivity.

*`Static`* version requires a lot of typing and no thinking, and adding *`interactivity`* requires a lot of thinking and not a lot of typing.

### Once you have a static application, what do you need to add ?
After building the static version of the app we have to make the UI interactive and that's by adding state to be able to trigger changes to your underlying data model.

### What are the three questions you can ask to determine if something is state ?

There are three main questions we have to think of to determine if something is state :
1. Is it passed in from a parent via props? If so, it probably isn’t state.
2. Does it remain unchanged over time? If so, it probably isn’t state.
3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

### How can you identify where state needs to live ?
React is all about one-way data flow down the component hierarchy. It may not be immediately clear which component should own what state. This is often the most challenging part for newcomers to understand, so we have to follow these steps to figure it out:

* Identify every component that renders something based on that state.
* Find a common owner component.
* Either the common owner or another component higher up in the hierarchy should own the state.
* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Higher-Order Functions :

### What is a “higher-order function” ?

**`Higher-order functions`** in JavaScript take some functions as arguments and return another function. They enable us to abstract over actions.

![Higher-order functions](https://pbs.twimg.com/media/EKT_82tXkAEuiqb.png)

### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing ?

```
function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// → true
```

Here in line 2 the **`greaterThan`** function is returinig an **`arrow`** function so the **`greaterThan`** function has **`Higher-order`** than the **`arrow`** function.

### Explain how either map or reduce operates, with regards to higher-order functions ?

Because **`map`** and **`reduce`** returens function in thier argument.

```
let newArray = array.map(element => element*element)
```
Here the map return function `element => element*element` so map has **`Higher-order`**.

![Higher-order](https://miro.medium.com/max/1400/1*bg8tKM_pfPOKa-Tfu3Uvow.png)