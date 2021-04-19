# Read: 12 - Docs for the HTML <canvas> Element & Chart.js

## Chart.js API
Charts are the best way to visualize data. They give information from the first look, and they are easy to read. Chart.js is a javascrip plugin that makes charts. Here are some information about it.
1.	Attach chart.js to html file ``` <script src='Chart.min.js'></script> ```
2.	Adding canvas element on the html file, chart.js will draw on this 
``` <canvas id="buyers" width="600" height="400"></canvas> ```
3.	 create a new _line_ chart: ``` new Chart(buyers).Line(buyerData); ```
4.	For the attributes of the chart, add them to an object. 
Some attributes: 
+ lables: [array];
+ fillColor
+ strokeColor
+ pointColor
+ pointStrokeColor
+ data [array]

There are other types of charts that can be created, like pie chart. 
## Canvas API
Canvas is an html tag that gives a space to draw on. It has only 2 attributes: width & height. It is a new tag, therefore, cannot be displayed in older browsers. But it is easy to overcome this, putting an alternative content inside it, the browser will display this alternative content and ignore the canvas tag. 
Canvas has a grid coordinate system that is used to determine positions. The origin point is the top left corner.
Canvas originally supports drawing only rectangles and paths. But you can use functions to draw more complex shapes.
