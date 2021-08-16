# Local Storage
## What is localStorage in JavaScript ?
localStorage is a property that allows JavaScript sites and apps to save key-value pairs in a web browser with no expiration date.
This means the data stored in the browser will persist even after the browser window is closed.

## How to Use LocalStorage ?
First we have to divide our topic to 4 main steps :
1. **`Saving our data to the localStorage.`**
2. **`Reading data from localStorage.`**
3. **`Clearing data from localStorage.`**
4. **`Removing item from localStorage.`**

### 1. **`Saving our data to the localStorage.`**
To save the data to the localStorage we use **`localStorage.setItem("key", "value")`**.
*`key`* is the name of this localStorage and *`value`* is the data we need to save.

Example :

```
let Arr = [1,2,3,4,5]
localStorage.setItem('array of numbers',Arr)
```

### 2. Reading data from localStorage.
To read the saved data from the localStorage we use **`localStorage.getItem("key")`**.
*`key`* is the name of the data we need to read from but here we need to asign it to a new variable.

Example :

```
let theValue = localStorage.getItem("Arr")
```

### 3. Clearing data from localStorage.
To clear all the data from the localStorage we use **`localStorage.clear()`**.
But be careful clear will delete all the data in the localStorage.

Example :

```
localStorage.clear()
```

### 4. Removing item from localStorage.
To remove only one item from the stored data we use **`localStorage.removeItem("key")`**.
*`key`* is the name of the data we need to remove, here we can specify the name of item we need to ramove.

Example :

```
localStorage.removeItem("Arr");
```