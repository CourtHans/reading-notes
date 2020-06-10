# Class 7 reading notes

**HTML & CSS** *Jon Duckett*

- Chapter 6: “Tables” (pp.126-145)

A ***table*** represents information in a grid format. Examples of tables include financial reports, TV schedules, adn sports results. 

The `<table>` element is used to add tables to a web page. A tabl3 is drawn out row by row, and in each row, there are data cells (or header cells, if appropriate).  You can use `rowspan` and `colspan`, and for long tables you can split the table into a `<thead>`, `<tbody>`, and `<tfoot>`.

<hr />

**JavaScript & JQuery** *Jon Duckett*

- Chapter  3: “Functions, Methods, and Objects” (pp.106-144)

The `new` keyword and the object constructor create a blank object. 

```
var hotel = new Object();
hotel.name = 'Quay';
hotel.rooms = 40; 
hotel.booked = 25;
hotel.checkAvailability = function() {
  return this.rooms - this.booked;
};
```

To create an empty object using literal notation, use: `var hotel = {}`  
The curly brackets create an empty object. So `var hotel = {}`  could be the same as `var hotel = new Object();`

When you have a value that is a string, you can use the properties and methods of the String object on that value. Each character in a string is given a number (**index number**).

### Six data types of JavaScript
*Simple*

1. **String**
2. **Number**
3. **Boolean**
4. **Undefined**
5. **Null**

*Complex*

6. **Object**

JavaScript has several built-in objects such as `String`, `Number`, `Math`, and `Date`. Their properties and methos offer functionality that help you write scripts. 

<hr />

Article:  
[Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an **object-oriented** model. A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. 

Building an efficient, clean, and functional model can deliver useful data for making decisions.

Object-oriented programming in JavaScript at its most fundamental level:
```
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```

1. The new keyword instantiates (i.e. creates) an object.
2. The constructor function initializes properties inside that object using the this variable.
3. The object is stored in a variable for later use.

Think of the **prototype** as an object's stunt double

**Reminder**: shared code means a running program consumes less memory which is important for devices like smart phones and tablets.

<hr />

[Previous - Class 6 reading notes](class-06.md) 
[Next - Class 8 reading notes](class-08.md) 

[Return to Table of Contents](README.md)