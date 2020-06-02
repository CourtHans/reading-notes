[Return to Table of Contents](README.md)

# Class 2 reading notes

**HTML & CSS** *Jon Duckett*

- Chapter 2: “Text” (pp.40-61)"
- Chapter 10: “Introducing CSS” (pp.226-245)

**Structural** and **Semantic markup**
Although HTML can be used to style text (*italics* or **bold**) for example, CSS should be the primary method for adding style to your page or site. The best use of HTML is to provide structure to your page. Even though some browers may style the text between semantic tags, semantic markup should be used to add extra information to your pages (e.g. information that would be useful for a screen reader).

**Structural markup examples**  
`<h1>` heading tag  
`<p>` paragraph tag  
`<sub>` subscript  
`<sup>` superscript  
`<br />` line break  (no closing tag needed)  
`<hr />` horizontal line break (no closing tag needed)

**Semantic markup examples**  
`<strong>` strong importance  
`<blockquote>` used for longer quotes (can use to cite source) though you can use `<cite>`  
`<abbr>` abbreviation (`<abbr title="insert full word here">`)  
`<dfn>` denote a defining instance  
`<s>` strikethrough - something that is no longer accurate (but that should not be deleted)

### CSS

CSS associates style rules wtih HTML elements.A CSS rule contains two parts: a selector and a declaration. A declaration sits inside curly brackers and has two parts, a property and a value (separated by a colon). 

`p {font-family: Arial;}`

`p` is the **selector**  
`{font-family: Arial;}` is the **declaration**  
`font family` is the property  
`Arial` is the value

**Using external CSS** (preferred for sites with more than one page) will require a `<link>` element (no closing tag needed) that lives inside the `<head>` element. It shoudl use 3 attributes: `<href>`, `<type>`, and `<rel>` (see p. 235).  
Example: `<link href="css/styles.css" type="text/css" rel="stylesheet" />`

**Using internal CSS** can be done with a `<style>` element (again, inside the `<head>`). The `<style>` element should use the type attribute to indicate that the styles are specified in CSS. The value should be `text/css`. (see p. 236)  
Example: `<style type="text/css">`

Examples of CSS selectors  
* Universal selector
* Type selector
* Class selector
* ID selector
* Child selector
* Descendant selector
* Adjacent sibling selector
* General sibling selector

***If there are two or more rules that apply to the same element, it is important to understand which will take precendence.***  (see pg 239)  
You can force a lot of properties to inherit values from their parent elements by using inherit for the value of the properties.

<hr />

**JavaScript & JQuery** *Jon Duckett*

- Chapter 2: “Basic JavaScript Instructions” (pp.53-84)
- Chapter 4: “Decisions and Loops” only up to the section on switch statements (pp.145-162)

Before you can use a variable, you need to announce that you want to use it. Create the variable and give it a name (**declare** the variable). Once created, you can **assign a value** to the variable.

There are three types of data:
1. numeric
2. string
3. boolean

**Naming variables** - must begin with a letter, $, or an _. **Must not** start with a number. The name can contain any of those things, as well as a number, but may not contain a `.` or a `-`. Use camelCase. Do not use keyworkds or reserved words. Be descriptive.

### Arrays

An array doesn't just store one value; it stores a list of values.

Example:  
`var colors;`  
`colors = ['white', 'black', 'custom'];`

The values are assigned to the array inside a pair of square brackets, each separated by a comma.  
Values in an array are accessed as if they are in a numbered list (starting at 0, not1).

### Functions, Methods, and Objects

In an object, variables are known as properties of the object; funtions are known as methods of the object.  
Flowcharts can help you plan for a script wherein decisions will be made that determine which lines of code will run. 

<hr />

[https://chris.beams.io/posts/git-commit/](https://chris.beams.io/posts/git-commit/)

> A well-crafted Git commit message is the best way to communicate context about a change to fellow developers (and indeed to their future selves).

Explain ***WHAT*** and ***WHY*** (this is not the place for HOW) so future you (and other developers) can follow the log.  A project's long term success depends upon (among other things) maintainability. A project log is a powerful tool to support this. Be clear, be concise.

### Seven rules of a great Git commit message

1. Separate subject from body with a blank line
2. Limit the subject line to 50 characters
3. Capitalize the subject line
4. Do not end the subject line with a period
5. Use the imperative mood in the subject line
6. Wrap the body at 72 characters
7. Use the body to explain *what* and *why* vs. *how*

[Previous - Class 1 reading notes](class-01.md)