# Week 2A - Review and more Canvas

## I. Overview
Today we will: 
- Take a look at the *ScreenSaver* submissions
- Answer any questions from last week
- (Here are some additional review questions about JS and the DOM - we don't have time to review all of them today - but you should look these over at some point --> [review-1.md](https://github.com/tonethar/IGME-330-Master/blob/master/notes/review-1.md))
- Talk about *Randomness & Aesthetics*
- Learn a little more about the Canvas API
- Refactor and add features to our screen savers

## II. Required Reading & Assignments (*see myCourses for due dates*)
<!-- - Shape Viewer HW -> [HW-shape-viewer.md](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-shape-viewer.md) -->
- This is a potential [Project 1 - *Interactive Sandbox*](../projects/project-1.md) "starter" --> [HW-Lorenz Attractor](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-lorenz-attractor.md)
- Study Guide-2 --> [HW-SG-2.md](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-SG-2.md)


## III. Extra Credit Opportunity (*see myCourses for due dates*)
- This is a potential [Project 1 - *Interactive Sandbox*](../projects/project-1.md) "starter" --> [HW-Random Walker](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-random-walker.md)

## IV. Presentations
- [Randomness and Aesthetics](https://github.com/tonethar/IGME-330-Master/blob/master/notes/randomness-1.md)
- [Canvas-2 More Canvas](https://github.com/tonethar/IGME-330-Master/blob/master/notes/canvas-2.md) - drawing rings, polygons, `ctx.arcTo()`, `ctx.lineJoin`, line dashes

## V. HW Assignment - *Screen Saver with Controls*
We will keep working on the Screen Saver:
- add a checkbox to control whether or not rectangles appear
- add **Pause** and **Play** buttons
- create a `drawRectangle()` helper function
- write code that "spray paints" rectangles onto the canvas when we click on it (e.g. like Jackson Pollock, but with digital rectangles instead)
- see videos "Screen Saver with Controls 1-4" below!
- see dropbox for due date

**Here's the HTML & CSS for the UI - for your copy/paste pleasure!**

```html
<section>
  <button id="playButton">Play</button> <button id="pauseButton">Pause</button>
</section>
<section>
  <span><input type="checkbox" id="rectanglesCB" checked><label for="rectanglesCB">Create Rectangles</label></span>
</section>
<section>
  <p>Click on the screen to "spraypaint" rectangles (you probably want the screensaver to be paused)</p>
</section>
```

```css
body{
  font-family: sans-serif;
}
	
canvas{
  border:1px solid gray;
}
	
button{
  font-size:1.2em;
}

section{
  margin:.5em 0 .5em 0;
}
```

**This helper code will come in handy when we want to determine where the user clicked on the canvas:**
```js
canvas.onclick = canvasClicked;

function canvasClicked(e){
  let rect = e.target.getBoundingClientRect();
  let mouseX = e.clientX - rect.x;
  let mouseY = e.clientY - rect.y;
  console.log(mouseX,mouseY);
}
```

## VI. Totally optional stuff you should do on your own

**\*\*Here are some optional (challenges) for you:\*\***

- add checkboxes to control the production of lines and circles
- create functions named `drawLine()` and `drawCircle()` (similar to `drawRectangle()` from the demo)
- create a `drawRing()` method that accepts an `innerRadius` and an `outerRadius` parameter (among others) and creates a ring like we did in Canvas-2 above.
- add a `linedash` parameter to `drawRectangle()`, `drawLine()` and `drawCircle()`, and utilize it if the developer passes in an array
- create a `drawTriangle()` function that accepts `width` and `height` parameters (among others) and draws a triangle like we did in Canvas-2 above

    
## VII. Reference
- https://developer.mozilla.org/en-US/docs/Web/API/CanvasRenderingContext2D

## VIII. Videos of lecture & demos

We aren't always going to have video links, but here is a re-cap of today's major topics:

- [Screen Saver With Controls-1 (12:33)](https://video.rit.edu/Watch/screen-saver-with-controls-1) - Adding a checkbox
- [Screen Saver With Controls-2 (06:53)](https://video.rit.edu/Watch/screen-saver-with-controls-2) - Adding Pause & Play buttons\*
- [Screen Saver With Controls-3 (14:01)](https://video.rit.edu/Watch/screen-saver-with-controls-3) - Creating a helper function 
- [Screen Saver With Controls-4 (08:59)](https://video.rit.edu/Watch/screen-saver-with-controls-4) - Adding mouse interaction

<hr>

The following two videos continue with the Screen Saver, and show you a technique for creating an external JS library using an IIFE - *Immediately Invoked Function Expression*. This is a requirement of Project 1. We will be covering this topic in class next week, but the video links are provided in case you are interested in learning this now:

- [Screen Saver With Controls-5 (22:06)](https://video.rit.edu/Watch/screen-saver-with-controls-5) - Getting rid of "magic numbers" and using an IIFE to remove our variables and functions from global scope
- [Screen Saver With Controls-6 (15:35)](https://video.rit.edu/Watch/screen-saver-with-controls-6) - Creating an ES5 Style JS Library with an IIFE

<hr><hr>

 \* ***If you code the Play button the way we did in the video, there's a problem. Click the Play button repeatedly and you'll see what the issue is. Go ahead and try to fix this - you can do so with just one line of code.***
 
<hr><hr>

| <-- Previous Unit | Home | Next Unit -->
| --- | --- | --- 
| [**week-01B-notes.md**](week-01B-notes.md)     |  [**IGME-330 Schedule**](../schedule.md) | [**week-02B-notes.md**](week-02B-notes.md)
