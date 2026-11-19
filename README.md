# Welcome to My Moving Box Realtime
***

## Task
/* What is the problem? */ 

The goal of this project is to animate an HTML element (`#my_box_realtime`) 
in real time using vanilla JavaScript so that it moves smoothly from its 
starting position (`right: 70px`, `bottom: 70px`) to the bottom-right corner 
(`right: 0px`, `bottom: 0px`) of the viewport.

/* where is the challenge? */
The main challenge is coordinating CSS positioning (`position: absolute`) 
with a JavaScript timer (`setInterval`), updating pixel coordinates 
accurately on each tick, and clearing the interval once the element 
reaches its destination to prevent memory leaks or unintended movement.

## Description
/* How have you solved the problem? */

I solved the problem by creating an `index.html` file inside `ex00/` 
containing a `100px × 100px` red `<div>` positioned absolutely 
at `right: 70px; bottom: 70px;`. 

In the `<script>` tag, I selected the element by its ID (`my_box_realtime`), 
initialized a position counter `pos = 70`, and used `setInterval()` 
to decrement `pos` by `1` every `500` milliseconds. On each step, 
both `box.style.right` and `box.style.bottom` are updated with `pos + "px"`. 
Once `pos <= 0`, `clearInterval(timer)` stops the animation.

## Installation
/* How to install your project? npm install? make? make re? */

No external dependencies or build steps are required. 

## Usage
/*  How does it work? */
```
To run the project locally, open `ex00/index.html` directly in any modern web browser:
```

### The Core Team


<span><i>Made at <a href='https://qwasar.io'>Qwasar SV -- Software Engineering School</a></i></span>
<span><img alt='Qwasar SV -- Software Engineering School's Logo' src='https://storage.googleapis.com/qwasar-public/qwasar-logo_50x50.png' width='20px' /></span>
