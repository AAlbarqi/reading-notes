# Chart.js, Canvas

**Chart.js** a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page.

The Steps of using Chart.js:
1. download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script:
`<script src='Chart.min.js'></script>`
2. Drawing a line chart: `<canvas id="buyers" width="600" height="400"></canvas>`
then Retrieve the context of the canvas: `<script>`
    `var buyers = document.getElementById('buyers').getContext('2d');`
    `new Chart(buyers).Line(buyerData);`
`</script>`
3. Drawing a pie chart: `<canvas id="countries" width="600" height="400"></canvas>` Next, we need to get the context and to instantiate the chart:
`var countries= document.getElementById("countries").getContext("2d");`
`new Chart(countries).Pie(pieData, pieOptions);`
after the pieData we’ll add our options:
`var pieOptions = {segmentShowStroke : false,animateScale : true}`
4. Drawing a bar chart: `<canvas id="income" width="600" height="400"></canvas>`
Next, we retrieve the element and create the graph:
`var income = document.getElementById("income").getContext("2d");`
`new Chart(income).Bar(barData);`
And finally, we add in the bar chart’s data.

##### [Here](https://www.chartjs.org/docs/latest/) is the documentation for chart.js

#### The canvas element : 
the <canvas> element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.
#### Drawing shapes with canvas
1. `fillRect(x, y, width, height)`
Draws a filled rectangle.
2. `strokeRect(x, y, width, height)`
Draws a rectangular outline.
3. `clearRect(x, y, width, height)`
Clears the specified rectangular area, making it fully transparent.
#### Drawing paths
- A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color.
To make shapes using paths, we take some extra steps:

1. First, you create the path.
2. Then you use drawing commands to draw into the path.
3. Once the path has been created, you can stroke or fill the path to render it.

#### Arcs
To draw arcs or circles, we use the arc() or arcTo() methods.

- `arc(x, y, radius, startAngle, endAngle, anticlockwise)`
Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise.
- `arcTo(x1, y1, x2, y2, radius)`
Draws an arc with the given control points and radius, connected to the previous point by a straight line.

#### Applying styles and colors
- `fillStyle = color`
Sets the style used when filling shapes.
- `strokeStyle = color`
Sets the style for shapes' outlines.
- `globalAlpha = transparencyValue`
Applies the specified transparency value to all future shapes drawn on the canvas. 
- `lineWidth = value`
Sets the width of lines drawn in the future.
- `lineCap = type`
Sets the appearance of the ends of lines.
- `lineJoin = type`
Sets the appearance of the "corners" where lines meet.
- `miterLimit = value`
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
- `getLineDash()`
Returns the current line dash pattern array containing an even number of non-negative numbers.
- `setLineDash(segments)`
Sets the current line dash pattern.
- `lineDashOffset = value`
Specifies where to start a dash array on a line.

#### Drawing text
The canvas rendering context provides two methods to render text:

- `fillText(text, x, y [, maxWidth])`
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- `strokeText(text, x, y [, maxWidth])`
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.