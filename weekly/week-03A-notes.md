# Week 3A - IIFEs and ES5 Style Libraries 


## I. Overview
- Review [HW-SG-1](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-SG-1.md):
  - look at "Smiley" submissions
  - concepts covered - this was mostly a review of what we have been doing in class (which is a good thing!)
- Review Periodic Functions & Phyllotaxis HW:
  - [HW - Sine Wave](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-sine-wave.md)
    - look at submissions
  - [HW - Algorithmic Botany](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-algorithmic-botany.md) 
    - look at submissions
- [Project 1](../projects/project-1.md) assigned! 
  - Let's discuss!
  - See dropboxes for due dates

## II. Lecture/Demo - the JavaScript IIFE
- Stands for "Immediately Invoked Function Expression"
- Using these is one of the requirements for Project 1
- See [IIFE Notes](https://github.com/tonethar/IGME-330-Master/blob/master/notes/IIFE-notes.md) & demo

## III. Demo - Modifying your "Screen Saver with Controls"
- Go ahead and grab your "Screen Saver with Controls" code from last week:
  - First, we'll re-factor the code by getting rid of ["magic numbers"](https://en.wikipedia.org/wiki/Magic_number_(programming)#Unnamed_numerical_constants) (e.g. Unnamed Numerical values or constants)
  - Next, we'll wrap all of our JS code in an IIFE
  - Then we'll create an ES5 style external "library" of reusable functions named **"abcLIB.js"** by using an IIFE (*abc* will be your initials):
    - time allowing, we'll also take a quick look at how RiTa.js structures their library using an IIFE: https://rednoise.org/rita/download.php


**Try it:** Once everything is working, move the remaining JS code in your HTML to an external JS file named **index.js**, and then import it with a &lt;script> tag


## IV. Videos
- These videos were originally linked to on 2A, and will re-cap what we covered in section III. above:
  - [Screen Saver With Controls-5 (22:06)](https://video.rit.edu/Watch/screen-saver-with-controls-5):
    - getting rid of "magic numbers" by adding `canvasWidth`, `canvasHeight` variables, and a `drawParams` object
      - https://en.wikipedia.org/wiki/Magic_number_(programming)
    - using `Object.freeze()` to create an [immutable object](https://en.wikipedia.org/wiki/Immutable_object)
    - using an IIFE ("immediately invoked function expression") to remove our variables and functions from global scope:
      - https://developer.mozilla.org/en-US/docs/Glossary/IIFE
  - [Screen Saver With Controls-6 (15:35)](https://video.rit.edu/Watch/screen-saver-with-controls-6):
    - Creating an ES5 Style JS Library with an IIFE

<hr><hr>

| <-- Previous Unit | Home | Next Unit -->
| --- | --- | --- 
| [**week-02B-notes.md**](week-02B-notes.md)     |  [**IGME-330 Schedule**](../schedule.md) | [**week-03B-notes.md**](week-03B-notes.md)
