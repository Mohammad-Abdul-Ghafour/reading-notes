# React and Forms
## Forms :

In React **`forms`** work a bit differently from HTML, because form elements naturally keep some internal state.

![Form](https://uxdt.nic.in/wp-content/uploads/2020/02/loginform1_p-1.png)

### Controlled Components :
In React, mutable state is typically kept in the state property of components, and only updated with **`setState()`**.

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input and this way is called a **`controlled component`**.

We should update the state with their responses as soon as they enter them, because the state will keep changing as user response changes.

We target user enters from the event it self by using **`event.target.value`**.

![Controlled Components](https://pbs.twimg.com/media/EKzwxZ4WkAAwjlw.jpg)

## Ternary Operator :
We use **`ternary operator`** to write **`if/else`** in one line.
For Example :

```
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

We can make it in one line as follows :

```
x===y? console.log(true) : console.log(false);
```