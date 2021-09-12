# State and Props

## React Lifecycle :

In React, components go through a lifecycle of events:

1. **`Mounting`**
2. **`Updating`**
3. **`Unmounting`**

![React Lifecycle Diagram](https://miro.medium.com/max/2000/0*0saPKFiTUk6W3FYp)

### What is the very first thing to happen in the lifecycle of React ? 

To understand React we should first know it's lifecycle. So the first thing happen in React lifecycle is **`Mounting`**, which consists of the code and React’s internals(*`Constructor`*), is then inserted into the DOM.

So *`Constructor`* is the very first thing happen in React lifecycle.

### Phases Call Order :

Based off the diagram in **`Mounting`** phase the following methods are called in order :

1. **`constructor`** :
    * The *`constructor`* is the very first method called as the component is brought to life.
2. **`getDerivedStateFromProps`** :
    * *`getDerivedStateFromProps`* is a new React lifecycle method as of React 17.
3. **`render`** :
    * *`render`* method is where you would write render elements to the DOM.
4. **`componentDidMount`** :
    * This function is invoked immediately after the component is mounted to the DOM.

` So render happens before componentDidMount`

5. **`React Updates`** :
    * This is the updating phase of the React component lifecycle.
6. **`componentWillUnmount`** :
    * The *`componentWillUnmount`* lifecycle method is invoked immediately before a component is unmounted and destroyed. This is the ideal place to perform any necessary cleanup such as clearing up timers, cancelling network requests, or cleaning up any subscriptions that were created in *`componentDidMount`* .

## Props Vs State :

### Props :
Think of props as arguments to a function.Typically when you have a piece of code that you would like to reuse, you can place that code into a function and any dynamic values that code used before can be accepted as argument.

For example :
```
const five = add(2, 3)
```
The same is true of a piece of JSX, except instead of calling it like a normal function you use JSX syntax
```
<Add n1={2} n2={3} />
```
So in props we can pass any type of data from parent to the child.

### State : 

State is data that changes over time, so precisely what React state is intended to be used for tracking data values over the lifetime of the component.

`So whenever the` *`state`* `changed we re-render the application.`

### So what is the big difference between props and state ?

**`Props`** can't be *`modified`* and *`read-only`*.

**`State`** can be *`modified`* and *`asynchronous`*.

![Props Vs State](https://i.stack.imgur.com/wqvF2.png)

#### Source :
* [LogRocket](https://blog.logrocket.com/react-lifecycle-methods-tutorial-examples/)
* [Kentcdodds](https://kentcdodds.com/blog/props-vs-state)