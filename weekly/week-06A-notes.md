<!--
# Week 6A - Intro to WebAudio API
-->

<!--
## I. Review
-->

<!--
- Any questions on last week's HW?
  - [Canvas VI - Sprites](https://github.com/tonethar/IGME-330-Master/blob/master/notes/canvas-6.md)
    - My preferred ES6 class technique:
      - (most) property names begin with an underscore as a convention indicating that they are *private* - ex. `_hitpoints`
      - the public accessor for the property is a "getter" method:
        - ex. `get hitpoints(){return this._hitpoints};`
      - the public mutator for the property is a "setter" method:
        - ex. `set hitpoints(value){value = parseInt(value); if(value >= 1) this._hitpoints = value; }`
      - see example below
  - [ES6 Module Pattern Notes](https://github.com/tonethar/IGME-330-Master/blob/master/notes/ES-6-module-pattern-2195.md)
    - also see this for "how to run your code off a web server" - because we'll need that again today (and for the entirety of the Project 2 unit)
- BTW - everyone knows how to set breakpoints in the browser debugger, right?
  - https://developers.google.com/web/tools/chrome-devtools/javascript/breakpoints

-->

<!--
## II. Presentation
-->

<!--
- [Web Audio I - Build a Simple Audio Visualizer](https://github.com/tonethar/IGME-330-Master/blob/master/notes/demo-web-audio-1.md)
- Helpful! [Web Audio Visualizer "Home" for IGME-330](https://github.com/tonethar/IGME-330-Master/blob/master/notes/web-audio-visualizer-home.md)
-->

<!--
## III. Homework Assignments
-->

<!--
See myCourses dropboxes for due dates:
  - [HW - Audio Visualizer - Part I](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-AV-2195-1.md)
  - [HW - Audio Visualizer - Part II](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-AV-2195-2.md)
  - [HW - Audio Visualizer - Part III](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-AV-2195-3.md)
--> 
 
<!--
## IV. Getter/Setter ES6 Class example
-->


# Week 6A - More JavaScript & Project 1 Crit Groups

## I. Review
- Any questions on ES6 Modules?
- Any questions on *transpiling*?

<hr>

## II. Project 1

- Any questions on the [Project 1](../projects/project-1.md) requirements?
  - The Project 1 Prototype is due Wednesday night 3/3/2021
  - The Project 1 Final Version is due Sunday night 3/14/2021
- Let's talk about the [Project 1 Crit Groups](p1-crit-groups.md)

<hr>

## III. Some more JavaScript

### III-A. JavaScript Getters and Setters

- What you do here is to create a "public property" that is actually going to call a setter method (where you could do data validation)
- You also need to create a "backing property", the convention is that it is the same name as the property but begins with an underscore
- You have probably seen this technique before in your C# classes
- BTW - this also works on object literals, not just classes

**setter-getter-tester.html**

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8" />
	<title>Setter Getter Tester</title>
</head>
<body>


<script>
		"use strict";
	class Monster{
		constructor(species,hitpoints){
			this._species = species;
			this._hitpoints = hitpoints;
		}
		
		// read-only
		get species(){
			return this._species;
		}
		
		get hitpoints(){
			return this._hitpoints;
		}
		
		set hitpoints(value){
			value = parseInt(value); 
			if(value >= 0) this._hitpoints = value;
		}
	
	}
	
	const m1 = new Monster("Orc",10);
	
	console.log(m1.species); 		// calls getter without parentheses
	console.log(m1.hitpoints); 	// calls getter without parentheses
	m1.hitpoints = 100 					// calls setter and passes in 100 for a `value`
	console.log(m1.hitpoints) 		
	m1.hitpoints = 2.6 					// calls setter and passes in 2.6 for a `value`, which is truncated to `2`
	console.log(m1.hitpoints) 
	m1.hitpoints = -300;				// calls setter and passes in -300 for a `value`, which is ignored
	console.log(m1.hitpoints)  
//	m1.species = "Goblin"; // ERROR!
//	m1._species = "Kobold"; // allowed! :-|
// console.log(m1.species); 
</script>
</body>
</html>
```
  
<hr>

## IV. Next time

- Sections 01 & 02 - Jefferson - traveling for the last time this semester - no Zoom meeting - instead there will be Slack office hours during the class time - a great time to stop in for questions or feedback on your Project prototypes:
  - before you leave - let's talk about the projects one more time
- Sections 03 & 04 - Wheeland - 

<hr><hr>

| <-- Previous Unit | Home | Next Unit -->
| --- | --- | --- 
| [**week-05B-notes.md**](week-05B-notes.md)     |  [**IGME-330 Schedule**](../schedule.md) | [**week-06B-notes.md**](week-06B-notes.md)
