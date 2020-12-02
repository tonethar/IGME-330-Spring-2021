# JS Debugging


## I. Debugging Concepts

- https://www.cs.cornell.edu/courses/cs312/2006fa/lectures/lec26.html

<hr>

## II. Debugging JavaScript

<hr>

## XXX. Homework

**Submission: copy the text below and paste it into a text editor, answer the questions, and ten export the file in PDF format (only) with a file name of *myLastname-myFirstname-debugging.pdf*, and then POST it to the myCourses dropbox prior to the due date:***

<hr>

**1) Read the article linked in part I. above and answer the following questions (by adding text to your *myLastname-myFirstname-js-fundamentals.html* file):**

1A) What advice does the author provide for *"... the best thing to do is ..."* ?

1B) Give an example of *defensive programming*

1C) Complete this sentence - *Remember, the goal is not to become an expert at fixing bugs, but rather to ...*

1D) List the 4 *"classes of defects"*

1E) Which one of these *"defects"* do you feel is generally the hardest to find and fix? (in a previous language you have used like C# or C++) Why?

**For the following questions we will look at *Debugging Strategies:***

1F) Describe ***Incremental and bottom-up program development***

1G) How would you ***Instrument program to log information*** in JavaScript?

1H) ***Instrument program with assertions*** is a good technique for "reality testing" while developing - JavaScript has `console.assert()` - described here: https://developer.mozilla.org/en-US/docs/Web/API/console/assert - and here's an example:

```js
let a = document.querySelector("#content");
console.assert(a !== null, "a is undefined!"); // program will halt here if a IS null (i.e. if the assertion fails)
a.innerHTML = "Welcome";
```

- The question you need to answer is, *What makes this a helpful debugging technique?*

1I) ***Use debuggers*** - What are the 2 ways you can set breakpoints in JavaScript programs?

1J) Define ***Backtracking***

1K) Explain ***Binary search***

1L) Give an example of ***Problem simplification***

<hr>




