# class 12

## Assorted bits of documentation:

### Read this [article](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/) on the Chart.js API

    Chart.js is a javascript plugin that lets you make fantastic looking charts

    You have to download the chart.js file folder through github
    Then paste the Chart.min.js file into the folder you are working in
    Import the script into the html and create a new chart in js

    < canvas id="name" width="600" height="400"></canvas> to create a canvas to start. pick width, height, and id

    Create a window into the DOM in javascript file

    Create a variable with data to finish rendering chart.
    Example from the article for simple line chart:

    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);

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

### [Chart.js docs](http://www.chartjs.org/docs/) You’ll be needing these

### Read the following articles on the Canvas API

    [Basic usage](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
        
        <canvas id="name" width="600" height="400"></canvas>  regular id tag with width and height

        Make sure to use closing tag
        
        Function to open window to a canvas and turn into 2d drawing template from article:
          function draw() {
        var canvas = document.getElementById('tutorial');
        if (canvas.getContext) {
          var ctx = canvas.getContext('2d');
        }
      }

    [Drawing shapes with canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)

      After canvas is created an

      Canvas only accepts two shapes, rectangles and paths

      fillRect(x, y, width, height)
          Draws a filledrectangle

      fillStyle = color
          Sets the style used when filling shapes.
      strokeStyle = color
          Sets the style for shapes' outlines.




    [Applying styles and colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)

      
    [Drawing text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)

       Function to draw text:   
          function draw() {
        var ctx = document.getElementById('canvas').getContext('2d');
        ctx.font = '48px serif';
        ctx.strokeText('Hello world', 10, 50);
      }
