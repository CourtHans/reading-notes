# Class 4 reading notes

**HTML & CSS** *Jon Duckett*

- Chapter 4: “Links” (pp.74-93)
- Chapter 15: “Layout” (pp.358-404) *special focus on 358-364

### Links

Links are creating using the `a` element. The destination is specified by the `href` attribute.
When linking to a page outside of yours, you'll use an absolute URL. Navigating to pages within your site will need a relative URL, taking note of the pathway through your directory. 

## Layout

Each HTML element has it's own "box."  
**Block-level** elements sstart on a new line  
**Inline** elements flow between surrounding text.

## Positioning schemes

* **normal flow**   (default behavior)  
* **relative positioning**  - moves an element from its 'normal' position (e.g. adjust with MBP)  
* **absolute positioning**  - positions element relation to its containing element. These will move as users scroll up and down the page.
* **fixed positioning** - form of absolute that positions the element in relation to browser window. Do not affect other elements, do not move when user scross up or down.
* **floating elements** - take element out of normal flow and position it to far left or right of container. Other elements will flow around it.

*When youmove any element from normal flow, boxes can overlap. The `z-index` property allows you to control which box appears on top.

***Because screen sizes and display resolutiosn vary so much, web designers often try to create pages of around 960-1000 pixels wide.***

Many designers try to let the user know what the site is about within the top 570-600 pixels, but don't try to cram too much into this top area.

<hr />

**JavaScript & JQuery** *Jon Duckett*

- Chapter  3 (first part): “Functions, Methods, and Objects” (pp.86-99)

**Functions let you group a series of statements together to perform a specific task. 

**Declaring a function**

```
function sayHello() {
  document.write('Hello!');
}
```
`function` is the keyword  
`sayHello()` is the function name  
the code block goes within the curly bracers `{}`

**Calling a function**  
Call (execute) the function by writing the cuntion name followed by parentheses.  
```
sayHello()
```

Functions can return more than one value using an array.

Ifyou declarea variable within a function, it can only be used within that function (variable's scope). 
Local variables take up less memory (page will be more responsive) and help avoid potential for naming conflicts.

<hr />

Article: [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

## Pair Programming

**Pair programming** helps Code Fellows students (developers) via the following 6 ways:
1. greater efficiency
2. engaged collaboration
3. learning from fellow students/developers
4. social skills
5. job interview readiness
6. work environment readiness

In paired programming, you will have a *Driver* and a *Navigator*.

<hr />

[Previous - Class 3 reading notes](class-03.md) 
[Next - Class 5 reading notes](class-05.md) 

[Return to Table of Contents](README.md)