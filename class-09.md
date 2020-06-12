# Class 9 reading notes

**HTML & CSS** *Jon Duckett*

- Ch 7: “Forms” (p.144-175)

When you need to collect information, you'll need to employe a form, designated by the `<form>` element. It will require a destination for the input and is sent in name/value pairs. Each type of form is given a name and the text the user types in or the values of the options they select and sent to the server. HTML5 has made these options more user friendly, providing ways for the script to validate type of entry (e.g. email, url). You can also provide keywords to clue your user in to what's expected.

- Ch 14: “Lists, Tables & Forms” (pp.330-357)

CSS allows you to take greater control over the appearance of lists, tables and forms, by (for example):

* Specifying the type of bullet point or numbering on lists
* Adding borders and backgrounds to table cells
* Controlling the appearance of form controls

You can customize the appearance of your lists with the `list-style-type` and `list-style` image properties.  
You can use CSS to make your tables and forms easier to read and give your user clues about how to interact with them. Forms are easier to use if form controls are vertically aligned with CSS.

Thoughtful design (as always) makes for a better user experience.

<hr />

**JavaScript & JQuery** *Jon Duckett*

- Chapter  6: “Events” (pp.243-292)

> WHen you browse the web, your browser registers different types of evens. It's the browser's way of saying, "Hey, this just happened." Your script can then respond to these events.

* Interactions create events
* Events trigger code
* Code responds to users

Events are said to ***trigger*** a script.  
When a user interacts with HTML on a web page, there are three steps involved in getting it to trigger; together these steps are known as **event handling**.  
1. Select **element**
2. Specify **event** 
3. Call **code**

Traditional DOM event handlers (*you can only attach one function to each event handler).  
`element.onevent = functionName;`  
`element` is the element
`oneevent` is the event (note: preceded by the word on)
`functionName` is the code

Event listeners can deal with more than one function at a time, but are not supported in older browsers. 

`element.addEventListener('event', functionName [, Boolean]);`

***Benefits fo Event Delegation***
* works with new elements
* solves limitations with this keyword
* simplifies your code

When calling a function, the event object's target property is the best way to determine which element the event occurred on (screen, page, client). 

Events are a browser's way of indicating when something has happened, upon which you can trigger a JavaScript function.

<hr />

[Previous - Class 8 reading notes](class-08.md) 
[Next - Class 10 reading notes](class-10.md) 

[Return to Table of Contents](README.md)