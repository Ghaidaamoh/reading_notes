# charts:

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going 
to press-gang them into use as a layout tool. A great way to get started with charts is with Chart.js,
a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. 

**Chart.js:**

- **Installation** You can get the latest version of Chart.js from npm , the GitHub releases , or use a Chart.js CDN .
  Detailed installation instructions can be found on the installation page.

- **Creating** a ChartIt's easy to get started with Chart.js. All that's required is the script included in
  your page along with a single **canvas** node to render the chart.

- **The canvas element** At first sight a **canvas** looks like the **img** element, with the only clear difference
 being that it doesn't have the src and alt attributes. Indeed, the **canvas** element has only two attributes, 
width and height. These are both optional and can also be set using DOM properties. When no width and height attributes 
are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily
by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio 
of the initial canvas, it will appear distorted.

**Drawing paths**
Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, 
curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes 
using paths, we take some extra steps:

- First, you create the path.
- Then you use drawing commands to draw into the path.
- Once the path has been created, you can stroke or fill the path to render it.

**Here are the functions used to perform these steps:**

1. **beginPath()** Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
2. **Path methods** Methods to set different paths for objects.
3. **closePath()** Adds a straight line to the path, going to the start of the current sub-path.
4. **stroke()** Draws the shape by stroking its outline.
5. **fill()** Draws a solid shape by filling the path's content area.

The first step to create a path is to call the beginPath(). Internally, paths are stored as a list of sub-paths
(lines, arcs, etc) which together form a shape. Every time this method is called, the list is reset and we can 
start drawing new shapes.

**Applying styles and colors**
there are two important properties we can use: fillStyle and strokeStyle.

**Drawing text**
The canvas rendering context provides two methods to render text:

- fillText(text, x, y [, maxWidth])
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.