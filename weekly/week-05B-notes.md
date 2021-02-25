# Week 5B - Transpiling Code / Project 1

## I. ES6 Modules

- Last time we covered ES6 Modules:
  - https://github.com/tonethar/IGME-330-Master/blob/master/notes/ES-6-module-pattern-2195.md
  - MDN [`import`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import)
  - MDN [`export`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/export)
  - Let's look at a completed example:
    - what does `import * as main from "./main.js";` import from **main.js**
    - in the above, **main** is a *namespace*, which makes it easier to keep track of where a function is declared. But, here we are only bringing in one function, so let's ditch the namespace. Try this instead:
      - `import {init} from "./main.js";`
      - and the all we have to do is to replace `window.onload = main.init;` with `window.onload = init;`
    - which style (namespace or no-namespace) is better to use? 
  - Any questions?

<hr>

## II. Transpiling 
- **What are the *advantages* of using ES6 modules?**
  - it allows many programmers to collaborate on the same application because a small team deals with only a small part of the entire code
  - the same code can be used in many applications
  - errors can easily be identified, as they are localized to a file, class or function
  - the scoping of variables can be easily controlled
- **What is the major *disadvantage* of using ES6 modules?**
  - They are only supported on modern browsers!

### II-A. Transpiling to the rescue!
 - https://github.com/tonethar/IGME-330-Master/blob/master/notes/node-and-transpiling.md
 - Ever heard the expression, "objects are for people"? It is an old phrase that means that the above advantages to using ES6 modules are important to developers, but ultimately the machine doesn't care if you write code with or without modules/objects etc

<hr>

## III. Project 1

- Any questions on the [Project 1](../projects/project-1.md) requirements?
- ***The discussion thread where you need to post your partner (optional) and idea (manadatory) closes tonight***
- The Project 1 Prototype is due Wednesday night 3/3/2021
- The Project 1 Final Version is due Sunday night 3/14/2021
- So, you need an idea!
- Possible themes:
  - Most of you are GDD students - so a game is appropriate - you can use "Sprity" as a starting point
  - An Audio Visualizer, or something that manipulates bitmap data, have been common projects in the past:
    - [Web Audio Visualizer - IGME-330 "Home Page"](https://github.com/tonethar/IGME-330-Master/blob/master/notes/web-audio-visualizer-home.md)
    - Bitmap Effect demos are on this page --> [Web Audio VI - Bitmap effects](https://github.com/tonethar/IGME-330-Master/blob/master/notes/demo-web-audio-6.md)
    - Machine Learning with *Teachable Machine*:
      - https://people.rit.edu/~acjvks/330/shared/machine-learning/teachable-machine/tm-1.html

<!--
- Are you sick of writing all of your JS code in one file and jamming everything into the global scope? ***You should be!***
- Today we are going to look at how to implement the *ES6 Module Pattern*:
  - [ES6 Module Pattern Notes](https://github.com/tonethar/IGME-330-Master/blob/master/notes/ES-6-module-pattern-2195.md)
- Note: One of the requirements of Project 2 is to utilize the *ES6 Module Pattern*
-->

<hr><hr>

| <-- Previous Unit | Home | Next Unit -->
| --- | --- | --- 
| [**week-05A-notes.md**](week-05A-notes.md)     |  [**IGME-330 Schedule**](../schedule.md) | [**week-06A-notes.md**](week-06A-notes.md)
