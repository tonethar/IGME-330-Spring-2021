# Week 1A: Course Introduction | JavaScript Review

Welcome to the course!

## I. Overview
Welcome to IGME-330 *Rich Media Web Application Development I*. In this "creative coding" course you will be building on top of IGME-230/235 and constructing compelling interactive experiences that can be viewed over the web. You will also be learning about how to build more robust and modular web software by utilizing more features of JavaScript ES6, with tools like Node.js and npm, and MVVM frameworks such as Vue.js


## II. Prerequisites
IGME-230 or IGME-235 is a pre-requisite, and you should have a solid understanding of these topics:
- HTML/CSS, and be able to post web files to `people.rit.edu` - if you forgotten how, [here are the instructions](https://github.com/tonethar/IGME-235-Shared/blob/master/notes/core-skills/ftp-upload-walkthrough.md)
- Basic JavaScript and the Web Browser DOM (Document Object Model)

### \*\*Important - Before class begins\*\*
- Review the topics in these ten [IGME-230/235 Web App tutorials](https://github.com/tonethar/IGME-230-Master/blob/master/notes/web-apps-0.md#section4) - most of this material should have been covered in your IGME-230 section. If you need a refresher on any of these topics, just go through the applicable tutorials at the link above. If you have any questions at all, or would like to have an assignment checked for accuracy, go ahead and reach out to me via email.


## III. Course Description & Topics
Official description from SIS: *This course provides students the opportunity to explore the design and development of Media Rich Internet Applications (MRIAs).  This course moves beyond client and server side web development, and explores issues of presentation, interactivity, persistence, and extensibility common among such applications.  Specifically, items explored include framework characteristics, data management, persistence, data binding, information manipulation, as well as data presentation.*


## IV. Pedagogy (how this course is taught!)
- ***You need to review the week's lecture notes *prior* to attending class for that week***
- A typical classroom day will be:
    - a review of the days topics (see the Github lecture notes)
    - a live demo by the professor that reinforces the day's topics
    - 2-way interaction (you could get called on at anytime)
- The assignments given in this class break into two categories:
    - homework assignments or in-class exercises that focus narrowly on one or more concepts
    - three projects with more flexible requirements that allow you to exercise considerable freedom and creativity in demonstrating key skills and understanding
- A large part of this course is taught similar to a typical math course: there will be several small homework assignments given every week, and because these assignments build upon one another, it is essential that they be completed both on-time and in-order, thus they have strict due dates.
- Keep an eye on the dropboxes in myCourses for what and when things are due. HW assignments will not be accepted late without prior permission from the instructor:
    - if something comes up and you need an extension for any reason, you need to get in touch with us at least 24-hours *before* the assignment is due
    - **Reminder:** *all code files (HTML, CSS, JavaScript) must be zipped when put in a dropbox, because otherwise myCourses strips out the JavaScript and CSS, and you will likely get a zero on the assignment*
- The due dates for these assignments will be clustered around the same days, often on Sunday night. This means that you should plan ahead, and not try to tackle them all in the last hour before they are due.
- Please get to class on time! Lectures will begin promptly at the start of class.

<hr>

***WEEK-0 COMMUNICATION***

- What name do you call me?
  - "Professor", "Professor Jefferson", or "Tony" all work
- Discord
  - Invites:
    - Change your nickname to your real name & section (ex. "Grace Hopper 01")
    - Post an Intro
  - Professional/SFW: Be aware of your status text (ex. "f-ing losing at Fortnight!" won't cut it)
- Zoom Professionalism
    - Article link (paywalled): https://www.wsj.com/articles/seven-rules-of-zoom-meeting-etiquette-from-the-pros-11594551601
    - The PDF of this article is in myCourses
    - Zoom - hold space bar to talk. But before you ask a question, first ask yourself "will others benefit from this question?"
      - if you are not sure they will, then post to the class Discord `#live-chat` channel
 - Participation/Engagement (10% of grade)
   - Zoom meetings
     - be on time (there's a waiting room for our Zoom meetings, so it's pretty obvious when someone is late)
     - keep web cam on, and microphone muted
     - you could get called on at anytime, so be ready to respond 
   - Discord Invite & Introduction & Logistics Survey
     - if I have to ask multiple times, it will hurt your participation grade
   - There will be several (graded) Discord discussion threads during the semester

      
***WEEK-0 ASSIGNMENT***

- *Technobabble* is due before we meet again - see myCourses dropbox
  - https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-technobabble.md

***WEEK-0 INTRODUCTIONS ("Do I have to?" - YES!)***
- Introductions - we'll do this alphabetically - so be ready:
 - 1) name/major/year
 - 2) where you are physically located right now
 - 3) your favorite food
 - 4) something interesting you did this summer
 - "Next!"

<hr>

## V. Required Reading & Assignments
* [syllabus.md](../syllabus.md)
* [schedule.md](../schedule.md)
* [Project 1 *Interactive Sandbox*](../projects/project-1.md) - this is what we are working towards for the first 1/3 of the course
* [Project 2 *Audio Visualizer* Showcase Video](https://video.rit.edu/Watch/Si56JxGd) - projects are shown starting at 5:00
* Keep an eye on the *Content* section of mycourses.rit.edu for "done" in-class demo files
* Keep an eye on the mycourses.rit.edu dropboxes to see what is assigned and when it is due

## VI. Starter Code

**starter.html**

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8" />
	<title>Starter Page</title>
	<style></style>
	<script></script>
</head>
<body>
<p>... something awesome goes here ...</p>
</body>
</html>
```

<a id="review-questions"></a>
 
## VII. Review notes and video on your own - JavaScript/DOM Review & Demo

- 1. What is JavaScript?
  - https://developer.mozilla.org/en-US/docs/Web/JavaScript
  - Used on both the client-side and server-side to create interactive web applications
  - Weakly typed:
    - after they are declared, variables can contain any type
    - JS uses *dynamic typing* to verify the type safety of a program at runtime, as opposed to compile time (static) typing
  - Multi-Paradigm:
    - *imperative* - a series of commands that describe how the program behaves (as opposed to *declarative* languages such as CSS or SQL)
    - *functional* - use functions to compose a program, avoid globals & mutable state
    - *event-driven* - program flow is driven by user and system events
    - *object-based* - an object literal, many built-in objects to use, and both prototypical and classical inheritance when the developer creates their own objects
    - *duck typed* - an object's suitability to be used for particular purpose is determined by the presence of certain methods and properties, rather than the type of the object itself
- 2. Setting up the development environment - easy!
  - A text editor
  - Chrome
  - create a web page, then run JavaScript in the console or type code into the &lt;script> tag
  - the console is an interactive **REPL** - "Read, Evaluate, Print, Loop"
    - shift-enter for multi-line code
    - up arrow to repeat last typed line
- 3. JavaScript Review & Demo
  - `'use strict';` - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode
  - declaring variables with `var`, `let`, and `const`
  - operators
  - data types:
    - `Boolean`, `Number`, `String`, `Null`, `Undefined`, `Symbol` (new for ES6) and `BigInt` (really new)
    - and `Object`
    - Reference: 
      - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures
      - https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects
  - Functions are also Objects and thus “first class” values, and can be both passed to functions and returned from them
  - `console.log()`
  - Standard built-in objects - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects
    - `Date`
    - `Math`
    - `Array`
  - Functions
    - writing functions
    - calling functions
    - Some DOM Elements (DOM = Document Object Model)
      - https://en.wikipedia.org/wiki/Document_Object_Model
      - https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model
    - Add &lt;button>, &lt;input>, and &lt;p>
    - Manipulating the properties of DOM elements:
      - `document.querySelector()`
      - `document.querySelectorAll()`
    - Events:
      - DOM elements have to load before we can manipulate their properties
      - event handlers - the `onclick` attribute
      - `element.addEventListener()`
- 4. JavaScript Debugger:
  - setting breakpoints
  - inspecting variable values 
  - viewing the call stack
  - "View Page Source" v. the Debugger's "Inspect Elements" view
- 5. Demo:
  - Add a "last name" input so that we can greet the person using both their first and last name
  - *Declaratively* (using CSS) make the button 50 pixels tall by 100 pixels wide
  - *Imperatively* (using JavaScript) give the paragraph a red text color, and a yellow background color

## VIII. Videos of JS & DOM Review demo

We aren't always going to have video links, but here they are in case we run out of time today:

<!---
- [Week 1A - JavaScript and DOM review - 1 (20:36)](https://video.rit.edu/Watch/f8H5Akr4) - the lecture begins at 8:50, the demo begins at 13:30 
- [Week 1A - JavaScript and DOM review - 2 (29:51)](https://video.rit.edu/Watch/Dr8n4XNz)
--->
- [JSReview-1: Using the console (06:18)](https://video.rit.edu/Watch/js-review-1-using-the-console)
- [JSReview-2: Variables and scope (16:12)](https://video.rit.edu/Watch/js-review-2-variables-and-scope)
- [JSReview-3: Working with DOM & Creating Greeter App (12:19)](https://video.rit.edu/Watch/js-review-3-working-with-dom-A)
- [JSReview-4: Working with DOM & Refactoring Greeter App (13:26)](https://video.rit.edu/Watch/js-review-4-working-with-dom-B)


## IX. Today's Activities

1) (This lecture is recorded) 
2) Questions from last time?
3) Questions on [Technobabble](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-technobabble.md)?
4) Quick Zoom Poll
5) Review some of the Part VII. notes above and create "Greeter" demo

**greeter-start.html**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Greeter</title>
    <style></style>
    <script></script>
  </head>
<body>
  <button>Click Me!</button>
  <input id="firstName" placeholder="Type in your name">
  <p id="output">???</p>
</body>
</html>
```
6) Begin [Canvas Paint HW - Part I](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-canvas-paint-app-1.md) - through Part VI. - see dropbox for due date          



<hr><hr>

| <-- Previous Unit | Home | Next Unit -->
| --- | --- | --- 
|   :-\  |  [**IGME-330 Schedule**](../schedule.md) | [**week-01B-notes.md**](week-01B-notes.md)
