# The canvas element

- the canvas will initially be 300 pixels wide and 150 pixels high.


```html
<canvas id="tutorial" width="150" height="150"></canvas>
```

## Accessing Rendering Context

 Rendering contexts method create canvas content .

 getContext() takes one parameter, the type of context

```js
var ctx = canvas.getContext('2d');
```

## Drawing in canvas methods :

## Colors (properties)

1. `fillStyle = color`

Sets the style used when filling shapes.

2. `strokeStyle = color`

Sets the style for shapes' outlines.


3. `globalAlpha =0.2` 

assigning transparency 

## Line styles
There are several properties which allow us to style lines. example:

- lineWidth = value
Sets the width of lines drawn in the future.
- lineCap = type
Sets the appearance of the ends of lines.


## create Pattern
we'll create a pattern to assign to the fillStyle property.

```
createPattern(img, 'repeat');
```

# CHART.JS

### - a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. 

### - makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy

### - first thing we need to do is download Chart.js. Copy the Chart.min.js 

<br>
<br>

## line chart

```js 
<script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>
```

```js 
var buyerData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "rgba(172,194,132,0.4)",
			strokeColor : "#ACC26D",
			pointColor : "#fff",
			pointStrokeColor : "#9DB86D",
			data : [203,156,99,251,305,247]
		}
	]
}
```

## Drawing shapes with canvas

- three functions that draw rectangles on the canvas:

```js
fillRect(x, y, width, height)
//Draws a filled rectangle.
strokeRect(x, y, width, height)
//Draws a rectangular outline.
clearRect(x, y, width, height)
//Clears the specified rectangular area, making it fully transparent.
```


## Drawing paths

`beginPath()`

Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.