# Class 12 reading notes

[Article on the Chart.js API](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)  
[Chart.js](https://www.chartjs.org/docs/latest/)  
[Basic usage](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)  
[Drawing shapes with canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)  
[Applying styles and colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)  
[Drawing text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)

Information presented visually leaves a far more powerful impression than information merely spoken or presented solely with words and numbers. Chart.js is a JavaScript plugin that can uses HTML5's canvas elements to bring in exciting visuals.

"At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties."

It's always a good idea to supply an ID to a canvas element. Also keep in mind it's a good idea to supply text descriptions to your canvas element for accessiblity and browser (in)compatibility reasons.

"The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. The `<canvas>` element has a method called `getContext()`, used to obtain the rendering context and its drawing functions. `getContext()` takes one parameter, the type of context. For 2D graphics, such as those covered by this tutorial, you specify `"2d"` to get a `CanvasRenderingContext2D`."

### Functions
`beginPath()` - Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.  
*Path methods* - Methods to set different paths for objects.  
`closePath()` - Adds a straight line to the path, going to the start of the current sub-path.  
`stroke()` - Draws the shape by stroking its outline.  
`fill()` - Draws a solid shape by filling the path's content area.  

There are two important properties we can use to impart color: fillStyle and strokeStyle. We'll use CSS color designates.

**`fillStyle = color`** - Sets the style used when filling shapes.  
**`strokeStyle = color`** - Sets the style for shapes' outlines.

You have to be very precise with pixels to get crisp looking lines. 

**`createPattern(image, type)`**  
"Creates and returns a new canvas pattern object. image is a `CanvasImageSource` (that is, an `HTMLImageElement`, another canvas, a `<video>` element, or the like. `type` is a string indicating how to use the image."

The canvas rendering context provides two methods to render text:

`fillText(text, x, y [, maxWidth])`  
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

`strokeText(text, x, y [, maxWidth])`  
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

<hr />

[Previous - Class 11 reading notes](class-11.md)  
[Next - Class 13 reading notes](class-13.md) 

[Return to Table of Contents](README.md)