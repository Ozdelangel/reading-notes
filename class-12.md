# Charts
- charts are easier to look at and convey data quickly
- You can use chart.js which is a plugin that uses html's canvas element to draw in the chart

Setting up
1. The first thing we need to do is download chart.js
2. copy the chart.min.js out of the unzipped folder and into the directory you will be working in
3. then create a new html file and import the script


Drawing a line chart
1. first thing we need to is create a canvas element in our html
2. add `<canvas id= "buyers" width='#' height="#"></canvas>` into the body of your html
3. we need to write a script that will retrieve the context of the canvas 
4. inside the same script tags we need to create our data, in this instance it's an object that contains labels for the bas of our chart and datasets to describe the values on the chart
### more on charts
- there are a few different types of charts you can create
- bar
- pie

# Basic Usage Of Canvas
- it kind of looks like the image tag without src and alt
- the canvas element only has to attributes width and height
# renderingg context
- the canvas is initially blank to display the element uses a method called `getContext()`