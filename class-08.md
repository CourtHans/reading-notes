# Class 8 reading notes

**HTML & CSS** *Jon Duckett*

- Ch. 15, “Layout” (again; repeat of Class 4 reading)  
[Sample layouts](http://htmlandcssbook.com/code-samples/chapter-15/)

**Normal flow** is static, **relative positioning** moves an element in relation to where it *would* have been in normal flow. **Absolute** positioning means the element will not longer affect the position of other elements on the page. **Fixed** position is what it sounds like... the object doesn't move as a user scrolls up or down. Z-indexes can be used to "bring to front/send to back" (PowerPoint parlance). 

**Float** position allows you to take an element and place it as far left or right in it's container as possible. 

***IF a container contains only floating elements***, some browsers will treat it as if it is zero pixels tall. The CSS solution to this is to give the container element an `overflow: auto;` property (with the `width: 100%` as well).

**Fixed width** layouts tend to be given in pixels.  
**Liquid** layouts tend to be given in percentages.

## Takeaway

When considering your layout - HAVE. A. PLAN. Even if it's just a pencil and paper sketch (low-fidelity) to get and keep you organized. This can help you write clean code from the beginning and ensure you have the proper html building blocks to execute your style via CSS.

<hr />

[Previous - Class 7 reading notes](class-07.md) 
[Next - Class 9 reading notes](class-09.md) 

[Return to Table of Contents](README.md)