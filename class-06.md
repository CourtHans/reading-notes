# Class 6 reading notes

**HTML & CSS** *Jon Duckett*

- Chapter 3: “Object Literals” (pp.100-105)
- Chapter 5: “Document Object Model” (pp.183-242)

### Object Literals

Objects group together a set of variable sand functions to create a model of something you would recognize from teh real world. 

In an object, variables become known as *parameters*.  
In an object, functions become known as *methods*.  
Properties and methods have a name and a value. In an object, that name is called a *key*.

```
var hotel = {
  naem: 'Quay',
  rooms: 40,
  booked: 25,
  checkAvailability: function () {
    return this.rooms - this.booked;
  }
}
```
The object is called *hotel*, the keys are *name*, *rooms*, *booked*, and *checkAvailability*. (The values follow each.) The properties are the first three, the method encompasses the function.

Separate each key from its value using a colon. Separate each property and method with a comma (but not after the last value [like after `this.booked`]). IN the above example, the `this` keyword is used to indicate that it is using the room sand booked properties of **this** object. 

You access the properties or methods of an object using dot notation. You can also access properties using square brackets.   
```
var hotelName = hotel.name;
var roomsFree = hotel.checkAvailability();

var hotelName = hotel['name'];
var roomsFree = hotel['checkAvailability']();
```

### Document Object Model

*The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.*

The DOM is called an object model because the model (the DOM tree) is made of objects. You will hear people call the DOM an **Application Programming Interface (API)**.  

Accessing and updating the DOM tree involves two steps:  
1. Locate the node that represents the element you want to work with.
2. use its text content, child element, and attributes.

The terms **elements** and **element nodes** are used interchangeably, but when people say the DOM is working with an element, it is actually working with a node that *represents* that element.

> Methods that find elements in the DOM tree are called DOM queries.

DOM queries may return one element, or they may return a NodeList, which is a collection of nodes. NodeLists look like arrays are are numbered like arrays, but they are not actually arrays; they are a type of object called a collection. Finding the quickest way to access an element within your web page will make the page seem faster and/or more responsive.

`get.ElementByID()` and `querySelector()` can both search an entire document and return individual elements. `querySelector()` is a more recent addition to the DOM, so not supported in older browsers. But it is flexible, which means it can be used to accurately target more elements.

There are two ways to select an element from a NodeList, both require the index number of the element you want.
1. The **item()** method
2. array syntax.

Array syntax is preferred because it is faster.
```
var elements = document.getElementsByClassName('hot');
if (elements.length >= 1) {
  var firstItem = elements[0];
}
```

`var elements = document.getElementsByClassName('hot');`  
Creates a NodeList containing elements that have a class attribute whose value is hot, and store it in the variable elements.

`if (elements.length >= 1)`  
If that number is greater than or equal to one, run the code inside the if statement.

`var firstItem = elements[0];`
Get the first element from the NodeList

**When you have a NodeList, you can loop through each node in the collection and apply the same statements to each.**

```
var hotItems = document.querySelectorAll('li.hot');
for (var i = 0; i < hotItems.length; i++){
  hotItems[i].className = 'cool';
}
```
`var hotItems = document.querySelectorAll('li.hot');`  
The variable **hotItems** contains a NodeList. It contains all the list items whose class attribute has a value of hot. They are collected using the querySelectorAll() method.

`for (var i = 0; i < hotItems.length; i++)`  
The length property of the NodeList indicates how many elements are in teh NodeList. The number of elements dictates how many times the loop should run.

`hotItems[i].className = 'cool'`  
Array syntax is used to indicate which item in the NodeList is currently being worked with: **hotItems[i]**. It uses the counter variable inside the square brackets.

<hr />

Article:  
[Understanding the problem domain is the hardest part of programming](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)

> "Writing code is a lot like putting together a jigsaw puzzle.  We put together code with the purpose of building components that we have taken out of the “bigger picture” of the problem domain."

The author argues that programming is easy if you understand the problem domain. He cites an example where he was "essentially given the entire problem domain in teh form of a spec that was clear and unambiguous," and states that - because of this - he was easily able to write the code.

It is exceptionally difficult to solve a problem before you know the question, therefore, **understanding the problem is the most critical piece to the equation."***  

Sometimes, to fully understand the problem domain, you need to parse it out to fully understand just one part. (Author cites games as being really good at this.)

### What to do?

> "Best to resist the temptation to “not waste anymore time talking” and make sure you understand a problem inside and out before you try and solve it with code.  It is much more expensive and time consuming to do things over than it is to do them right the first time.  I learn this lesson the hard way time and time again."

***Take your time to REALLY understand the problem, talk it out, and go in-depth BEFORE you write a single line of code.***


<hr />

[Previous - Class 5 reading notes](class-05.md) 
[Next - Class 7 reading notes](class-07.md) 

[Return to Table of Contents](README.md)