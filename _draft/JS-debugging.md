# JS Debugging

- Do you ALWAYS write perfect code that runs flawlessly the first time you test it? Neither do we!
- Today we are going to discuss debugging techniques we can use with the JavaScript programs we will write for this class

<hr>

## I. Code Debugging Concepts

- If the output or behavior of a program is not what the developer expected, then the program is incorrect -- it contains ***errors*** (aka ***bugs***)
- This testing reveals the existence of programming errors, but not the cause of errors. The programmer must then go through a *debugging process* in order to be able to identify the causes and then fix the errors:

- READ: https://www.cs.cornell.edu/courses/cs312/2006fa/lectures/lec26.html

<hr>

## II. Debugging JavaScript

- READ and WATCH: Google Chrome Debugger: https://developers.google.com/web/tools/chrome-devtools/javascript (video embedded at top)

<hr>

## XXX. Homework

**Submission: copy the text below and paste it into a text editor, answer the questions, and then export the file in PDF format (only) with a file name of *myLastname-myFirstname-debugging.pdf*, and then POST it to the myCourses dropbox prior to the due date:***

<hr>

**1) Read the article linked in part I. above and answer the following questions:**

1A) What advice does the author provide for *"... the best thing to do is ..."* ?

1B) Give an example of *defensive programming*

1C) Complete this sentence - *Remember, the goal is not to become an expert at fixing bugs, but rather to ...*

1D) List the 4 *"classes of defects"*

1E) Which one of these *"defects"* do you feel is generally the hardest to find and fix? (in a previous language you have used like C# or C++) Why?

1F) Give an example of a *"defects"* that most frequently ends up in your code:

**For the following questions we will look at *Debugging Strategies:***

1G) Describe ***Incremental and bottom-up program development***

1H) How would you ***Instrument program to log information*** in JavaScript?

1I) ***Instrument program with assertions*** is a good technique for "reality testing" while developing - JavaScript has `console.assert()` - described here: https://developer.mozilla.org/en-US/docs/Web/API/console/assert - and here's an example:

```js
let a = document.querySelector("#content");
console.assert(a !== null, "a is undefined!"); // program will halt here if a IS null (i.e. if the assertion fails)
a.innerHTML = "Welcome";
```

- The question you need to answer is, *What makes this a helpful debugging technique?*

1J) ***Use debuggers*** - Give 2 ways you can set breakpoints in JavaScript programs:

1K) Define ***Backtracking***

1L) Explain ***Binary search***

1M) Give an example of ***Problem simplification***

1N) Give an example of ***A scientific method: form hypotheses***

1O) What is ***Bug clustering***?

1P) We will talk about ***Error-detection tools*** in the next section (*no answer required*)

1Q) Note two of the additional strategies that were suggested (*no answer required*):

- *The bug may not be where you expect it.* It a large amount of time has unsuccessfully been spent inspecting a particular piece of code, the error may not be there. Keep an open mind and start questioning the other parts of the program.
- *Make sure you have the right source code.* One must ensure that the source code being debugged corresponds to the actual program being run ... (WE SEE THIS ALL THE TIME)

<hr>




