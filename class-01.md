[Return to Table of Contents](README.md)

# Class 1 reading notes

### HTML

**HTML & CSS** *Jon Duckett*

- Introduction (pp.2-11)
- Chapter 1: “Structure” (pp.12-39)
- Chapter 8: “Extra Markup” (p.176-199)
- Chapter 17: “HTML5 Layout” (pp.428-451)
- Chapter 18: “Process & Design” (pp.452-475)

**Tags** act like containers, telling you something about the information that lies between their opening and closing tags. `<p>` is an example of an opening tag, and the corresponding closing tag looks like this - `</p>`.

**Attributes** provide additional information about the contents of an element. For example, 

`<p lang="en-us">Paragraph in English</p>`

The attribute name, `lang` indicates what kind of extra information is supplied.  The value, `"en-us"` is the setting of the attribute (and should be placed in double quotes). MOst atrribute values are either pre-defined or follow a stipulated format.

The `<head>` element contains information *about* the page (rather than information that is shown within the main part of the browser). You will usually find a `<title>` element inside the `<head>` element.

### Extra Markup

Because there hae been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browswer which version of HTML the page is using, such as `<!DOCTYPE html>`. 

If you want to add a comment to your code that will not be visibile in the user's browser, you can do this: `<!-- comment goes here -->`. Comments within your code can help you (or other people) when you come back later.

* **ID attributes** - used to uniquely identify the element from other elements on the page. Its value should be unique and start with a letter or an underscore. E.g. `<p id="pullquote">`
* **Class attributes** - a way to identify several elements as being different form the other elements on the page. E.g. `<p class="important">`. If you would like to indicate that an element belongs to several classes, you can separate class names with a space.
* **Block elements** - Some elements will always appear to start on a new line in the browser window. Examples are `<h1>, <p>, <ul>,` and `<li>`.
* **Inline elements** - In contrast, some elements will always appear on the same line. Examples are `<a>, <b>, <em>,` and `<img>`.
* **`<div>`** - this elemet allows you to group a set of elements together in one block-level box. Using an id or class attribute on the `<div>` element means you can create CSS style rules to indicate how much space the element should occupy, change the appearance, etc. It can also make it easier to follow your code.
* **`<span>`** - this element acts like an inine equivalent of the `<div>` element. It is used to contain a section of text or a number of inline elements. Again, used with CSS.
* **`<iframe>`** - a little windown that has been cut into your page (think Google maps). Youll also need `src` attribute, `height` attribute,`width` attribute.
* **`<meta>`** - lives inside the `<head>` element and contains info about that web page. NOt visible to users. Does not have a closing tag.

Headers, footers, navigation, articles, sections, asides, figures, heading groups, etc. can and should be used to provide clearer code (compared with using multiple `<div>` elements).

When designing your site, it is critical to think about your user's perspective. **WHO** is it for, **WHY** are they visiting, **WHAT** are they trying to achieve and what informatio do they need, and **HOW OFTEN** will they visit your site? An exercise such as *card sort* can help you think about how to organize your page, and a *wireframe* is a simple sketch of the key information that needs to go on each page of the site (shoing hierarchy and spatial requirements).

> It can be helpful to show a client the wireframes of a site before showing them a design. It enables the client to ensure the site has all the functions and information it needs to offer.

***REMEMBER***, the primary aim of any kind of visual design is to communicate.

Designing navigation...Good navigation tends to follow these principles: 
1. **concise**
2. **clear**
3. **selective**
4. **context**
5. **interactive**
6. **consistent**

### JavaScript

**JavaScript & JQuery** *Jon Duckett*

- Introduction
- JS Chapter 1: “The ABC of Programming” (pp.11-52)

>As tempting as it can be to start coding straight away, it pays to spend time designing your script before you start writing it.

A script is a series of instructions that the computer can follow in order to achieve a goal. To approach writing a script, break down your goal into a series of tasks, then work out each step needed to complete that task.

Computers use data to create models of things in the real world. Events can trigger methods, and methods can retrieve or update an object's properties.

Objects can have properties, methods, and events.

`<html>` is the content layer, `{css}` is the presentation layer, and `javascript()` is the behavior layer.

`document.write('Good afternoon!');`

- `document` is the object
- `.` is the member operator
- `write();` is the method
- `'Good afternoon!'` is the parameter

It is bets to keep JavaScript code in its own file.

[Next - Class 2 reading notes](class-02.md)