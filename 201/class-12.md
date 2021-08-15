# Chart.js API :
**`Chart.js`** comes with the following built-in chart types:

* **`Scatter`**

    ![Scatter chart](https://wisej.com/wp-content/uploads/2016/05/chartjs_scatter_chart.png)

* **`Line`**

    ![Line Chart](https://forum.vuejs.org/uploads/default/original/1X/25c3da357dc92766894445454e4e8df55db38a84.png)

* **`Bar`**

    ![Bar Chart](https://miro.medium.com/max/1838/1*s9ACgOrgGMCCwQKf-p88sQ.png)

* **`Radar`**

    ![Radar Chart](https://user-images.githubusercontent.com/32865180/32367314-fbdd33f4-c081-11e7-8a2b-b54ea0d69f9e.png)

* **`Pie and Doughnut`**

    ![Pie Chart](https://i.stack.imgur.com/uyehv.png)

* **`Polar Area`**
    
    ![Polar Chart](https://wpdatatables.com/wp-content/uploads/2020/12/Chart.js-Polar-Chart.jpg)

* **`Bubble`**

    ![Bubble Chart](https://datasciencepr.com/wp-content/uploads/2020/06/bubble_chart.png)

## How to Use Chart.js ?
Chart.js is easy to use.
1. First, add a link to the providing CDN (Content Delivery Network):

```
<script
src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.9.4/Chart.js">
</script>
```

2. Then, add a **`<canvas>`** to where you want to draw the chart:

```
<canvas id="myChart" style="width:100%;max-width:700px"></canvas>
```
The canvas element must have a unique id.

And that's all of how to use chart.js.

## Canvas API :
The HTML **`<canvas>`** tag is used to draw graphics, on the fly, via scripting (usually JavaScript).
### What Canvas Can Do ?
1. Canvas Can Draw Text : Canvas can draw colorful text, with or without animation.

2. Canvas Can Draw Graphics : Canvas has great features for graphical data presentation with an imagery of graphs and charts.

3. Canvas Can be Animated : Canvas objects can move. Everything is possible: from simple bouncing balls to complex animations.

4. Canvas Can be Interactive : Canvas can respond to JavaScript events.

5. Canvas Can be Used in Games : Canvas' methods for animations, offer a lot of possibilities for HTML gaming applications.

### Drawing shapes with canvas :
**`<canvas>`** only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.

First let's look at the rectangle. There are three functions that draw rectangles on the canvas:

1. **`fillRect(x, y, width, height)`**
    * Draws a filled rectangle.
2. **`strokeRect(x, y, width, height)`**
    * Draws a rectangular outline.
3. **`clearRect(x, y, width, height)`**
    * Clears the specified rectangular area, making it fully transparent.

Example :

```
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}
```

This example's output is shown below.

![Drawing shapes with canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes/canvas_rect.png)