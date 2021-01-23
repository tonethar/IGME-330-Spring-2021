# Week 1B - More JavaScript Review

## I. Overview

- Welcome to day 2! 
- First we'll see if there are any questions about the Technobabble HW, and take a peak at a few submissions
- Then we will continue our review of basic JavaScript and the DOM, and cover the material in the third and 4th videos from last time:
  - see the [Week 1A - JS review notes](week-01A-notes.md#js-review-notes)
  - and [Week 1A - JS review videos](week-01A-notes.md#js-review-video-links)
  - if we don't get to cover all of this material during the class time, you are expected to get this material by watching the video links at the bottom of this page
  - here is the start code for today's demo (and Homework)

**say-hello-2.html**
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Greeter</title>
    <style>
      *{font-size:1.5em;}
    </style>
    <script>
    'use strict';
    </script>
  </head>
<body>
  <button>Click Me!</button>
  <input id="firstName" placeholder="Type in your name">
  <p id="output">???</p>
</body>
</html>
```



## II. Homework
- Easy!
- Take the final version of what we created in the last video (the **say-hello-3.html** file):
  - Change the "Click Me" button text to "Hello" 
  - Add a "Last Name" field the user can type into
  - When the user clicks the "Hello" button they will greeted with both their first and last name
  - If no value is entered for the "Last Name", the default value will be "Bond"
  - Add a second button with the text of "Goodbye"
  - When the user clicks the "Goodbye" button, it will function nearly identical to the "Hello" button, except it will display "Goodbye `<firstName>` `<lastName>`"
  - See screenshot below

![screenshot](_images/1B-hello-goodbye.png)

- see myCourses dropbox for due date


<hr><hr>

| <-- Previous Unit | Home | Next Unit -->
| --- | --- | --- 
| [**week-01A-notes.md**](week-01A-notes.md)     |  [**IGME-330 Schedule**](../schedule.md) | [**week-02A-notes.md**](week-02A-notes.md)
