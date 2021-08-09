# CSS Layout
## What is CSS Layout :
CSS page layout techniques allow us to take elements contained in a web page and control where they're positioned.

For example like in this image below :

![CSS Layout](https://cdn.codecoda.com/themes/user/site/default/asset/img/blog/CSS-layout-1.png)

In this image we can see that we positioned each HTML tag where we need them to be.

### Then how to do that :
We to that by useing `position` property with the value we need.

And there are 5 main value and thay are :
* **Static**
* **Relative**
* **Absolute**
* **Fixed**
* **Sticky**

#### Static Positioning :
Static positioning is the default value for all tag. It just puts the element into its normal position in the document layout flow.

*EX* :

```
div {
  position: static;
}
```

#### Relative Positioning :
Relative positioning it's similar to static positioning but in but here we can edit it position by given it `left` `right` `top` `bottom`.

*EX* :

```
div {
  position: relative;
  top: 30px;
  left: 16px;
}
```

#### Absolute Positioning :
 Absolute positioning it takes the element out of normal flow and no longer affects the position of other elements on the page. Also we can edit it position by given it `left` `right` `top` `bottom`.

 *EX* :

```
div {
  position: absolute;
  top: 30px;
  left: 16px;
}
```

#### Fixed Positioning :
Fixed positioning usually fixes an element in place relative to the visible portion of the viewport.

 *EX* :

```
div {
  position: fixed;
  height: 1400px;
}
```

#### Sticky Positioning :
Sticky positioning is basically a hybrid between relative and fixed position, which allows a positioned element to act like it is relatively positioned until it is scrolled to a certain threshold point.

*EX* :

```
div {
  position: sticky;
  top: 30px;
  left: 30px;
}
```

## Z-Index Property :
`z-index` is a reference to the `z-axis`. `z-axis` an imaginary line that runs from the surface of your screen, towards your face. Then `z-index` values affect where positioned elements sit on that axis.

## Float Property :
Float property takes the element and place it as far to the left or right of the containing element as possible. 

## Clear Property : 
Clear property allows you to say that no element should touch the left or right sides of a box.

And it takes 4 values :
* left
* right
* both
* none

*EX* :

```
div {
    clear: left;
}
```

## @Import :
@import rule tells the CSS engine to import an external style sheet into another style sheet. This allows style rules from a style sheet to be added to another style sheet. This rule can also be used in combination with media queries to import a style sheet based on the device type.

`@import "style.css";`