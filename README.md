# jquery.flot.addTitle.js
Adds a title to the canvas of a plot.

## Installation
Just include the jquery.flot.addTitle.js after you've included jquery.flot.js.

Example:

``` html
<script src='/flot/jquery.flot.addTitle.js'></script>
```

## Usage
To set the title of the graph, the option needs to be enabled under options, grid. The default options for addTitle are as follows:
``` javascript
options = {
    grid: {
        title: {
            show: false,
            font: '12px sans-serif',
            color: 'black',
            text: 'This is a Title',
            delimiter: ' ',
            interLineSpacing: 6
        }
    }
}
```
#### show
Set show to true in order to display the title.

#### font
**IMPORTANT: Font size must be in px, and must be listed first!**

Set the font of the title.

#### color
Set the text color of the title.

#### text
The actual text that comprises of the title.

#### delimiter
The word wrapping function will use the delimiter to break up the title into segments. The word wrapping function will continually add segments to one line until the title would be larger than the grid, and then will start adding segments to the next line. Use a delimiter other than space if your title contains a repeating delimiter in your title.

Example:
``` javascript
title: "First_Name: John | Last_name: Smith | Gender: Male",
delimiter: " | "
```
Would result in three segments:
``` javascript
"First_Name: John",
"Last_Name: Smith",
"Gender: Male"
```
