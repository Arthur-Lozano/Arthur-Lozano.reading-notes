# Creating stunning animated charts with chart.js

- Charts are better to display data than a table
- chart.js is a javascript plugin and is a great way to get started with charts

*Chart.js
- Uses HTML5's canvas element to draw the graph onto the page.
- Can make various types of charts such as (pie, line, bar, and more with ease)

*Main points to set up a chart

- Connect the chart.js to your html page
- Create a canvas element within our HTML in order for chart.js to draw charts on
- Write a script that will retrieve context from canvas (such as the document.getElementbyId)
- Within the same script tags that we got our element by ID we need to create our data.  Perhaps an object that contains labels for the base of whatever charts are created and datasets to describe the values on the chart.

# `The <canvas> element`

- Has only two attributes (Height and Width)
- When these attributes are not set the default is (300px by 150px)
- It is good practice to utilize the `id` attribute because it makes the canvas easier to identify within a script

* It is important to display fallback content for older browsers that cannot display the canvas
* Scripts can also check for support programmatically by testing for the presence of the `getContext` method

# The rendering context

- `getContext()`, takes one parameter, such as '2d' (used to obtain the rendering context and its  drawing functions)

# Drawing shapes with canvas

* The grid/coordinate space
- Usually one unit in the grid corresponds to one pixel
- Origin of the grid is positioned in the top left corner at coorindate (0,0)
- All elements are placed relative to this origin
- canvas only supports two primitive shapes: rectangles and paths.  Any other shapes must be created by combining one or more paths.

* There are an assortment of path drawing functions at our fingertips that allow us to draw compose very complex shapes.

### Drawing paths

- A path is a list of points connected by segments of lines that can consist of different curves, shapes, widths, and even color.

* Below are functions to draw paths

-`beginPath()`
-Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.

- `Path methods`
Methods to set different paths for objects.

- `closePath()`
- Adds a straight line to the path, going to the start of the current sub-path.

- `stroke()`
- Draws the shape by stroking its outline.

- `fill()`
- Draws a solid shape by filling the path's content area.

## Applying styles and colors

- If we want to apply color to a shape there are two properties we can use (fillStyle and strokeStyle)

### Other visual tools 

- Transparency (`globalAlpha`)
* Line styles
-lineWidth = value
-Sets the width of lines drawn in the future.
-lineCap = type
-Sets the appearance of the ends of lines.
-lineJoin = type
-Sets the appearance of the "corners" where lines meet.
-miterLimit = value
-Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
-getLineDash()
-Returns the current line dash pattern array containing an even number of non-negative numbers.
-setLineDash(segments)
-Sets the current line dash pattern.
-lineDashOffset = value
-Specifies where to start a dash array on a line.

- lineWidth
- lineCap
- lineJoin

## Drawing text

* The canvas rendering context provides two methods to render text 
- fillText
- strokeText

## Styling text

- font = value
- textAlign = value
- textBaseline = value
- direction = value

## Advanced text measurements

- measureText()

ref: https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/
ref: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage
ref: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes
ref: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors
ref: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text

