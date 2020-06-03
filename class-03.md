# Class 3 reading notes

**HTML & CSS** *Jon Duckett*

- Chapter 3: “Lists” (pp.62-73)
- Chapter 13: “Boxes” (pp.300-329)

### Lists
Ordered lists are numbered, unordered lists are bulletted - each next within either a `<ol>` or `<ul>` tag, with each list item tagged with a `<li>` tag.  
You can put a second list inside an `<li>` element to create a sub-list or nested list.
```
<ul>
   <li>Monday
     <ul>
       <li>Breakfast: crepes</li>
       <li>Lunch: pb&j</li>
       <li>Dinner: burrito bowls</li>
     <ul>
   </li>
   <li>Tuesday
     <ul>
      <li>Lunch: soup</li>
      <li>Dinner: salad</li>
     <ul>
   </li>
</ul>
```
A **Definition list** offers additional formatting and is created within the parent tag `<d1>`. The `<dt>` tags contain the terms being defnined, and the `<dd>` tags contain the definitions.

### Boxes
CSs treats each HTML element as if it has its own box. With CSS, we can control the appearance of the page through box manipulation/styling (borders, width, height, visitiliby, etc.)

By default, a box is sized just big enough to hold its contents. You can change the demnsions with specifications around: *pixels*, *percentages*, and *ems*. Percentages will affect the size of the box in rleation to the size of the browser window (more responsive styling). `<min-width>`, `<max-width>`,`<min-height>` and `<max-height>` are also useful for screen size adjustment.  
The **overflow** property tells the browswer what to do if the content contained within a box is larger than the box itself. It can hide overflow (*hidden*) or add a scrollbar (*scroll*). (p. 306)

> Every box has three available properties that can be adjusted to control its appearance: **border**, **margin**, and **padding**.

You can control border styles (i.e. dash, ridged, inset), width (thin, thick, 3px), and color. You can style each part seperately, but the border property allows you to coe in one expression. It's important to keep it in the order of width, style, and color.

Example:  
```
p {
  width: 250px; border: 3px dotted #008dd;}
```
**Padding** is added onto the width of the box, and can make text easier to read wthin a bordered element. **Margin** properties control the gap in between boxes. Padding and margin shorthand will let you adjust your padding in clockwise order: top, right, bottom, left):

Example:  
```
padding: 10px 5px 3px 1px;
margin: 1px 2px 3px 4px;
```
or
```
padding: 20 px 10px;
margin: 15 px 30px;
```
The latter example  assigns the top and bottom margins first (20px for padding, 15 px for margin) and the left & right second (10px for padding, 30px for margin).

If you want to center ab o on the page (or w/in an element) you can set the left-margin and right-margin to auto, but ou will need to set a width for the bo (or it will take up the full width of the page).

**Change inline/block**  
One way to create navigation across your page is to take a list and display it inline (with a margin-right to space them out).

Example:
```
li {
  display: inline;
  margin-right: 10px;}
```
You can also fully hide an element (p 318) with the visibility property (values are *hidden* or *visible*).

**Box shadows** (p320) can be used to add a drop shadow around a box, and include a horizontal offset, vertical offset, blur distance, and spread of shadow.

**Border-radius** can create rounded corners and elliptical shapes (p322).

<hr />

**JavaScript & JQuery** *Jon Duckett*

- Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)

A **switch** statement starts with a variable called the **switch value**.  A break statement will stop the code once a match has been found, therefor running more quickly than and if...else statement. (p 164)

JavaScript can convert data types behind the scenes to complete an operation (like string into a number, changing cases). This can make for a much better user experience.

### Loops

Loops check a condition; if it returns true, a code block will run. There are **for**, **while**, and **do while** loops.  
A **for loop** uses a counter as a condition and is made up of an initialization, condition, and update statement.

The `+=` operator is used to add new content to the msg variable.

[Previous - Class 2 reading notes](class-02.md)  
[Next - Class 4 reading notes]()

[Return to Table of Contents](README.md)