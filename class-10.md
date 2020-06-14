# Class 10 reading notes

**JavaScript & JQuery** *Jon Duckett*

- Ch. 10, “Error Handling & Debugging”

Understanding execution contexts (when will something run)/order of operation in your code, you are more likely to find your errors. Debugging calls upon your powers of deduction, and sometimes fellow developers/coders/colleagues. It can be helpful to either narrate what your code is doing to a colleague or - failing another set of ears - talk through your code out loud. This is referred to as "explaining the code". 

### Tips

* Check another browser
* Add numbers/write them into the console to see which items get logged
* Strip it back - take out pieces of your code down to the minimum to see what DOES run without error
* Explain the code 
* Search the web!
* Coding communities - post your problems and crowdsource solutions
* Validation tools

Common mistakes include case-sensitivity errors, missed/extra characters, and data types. 

JavaScript has 7 different types of errors: 
1. SyntaxError
2. ReferenceError
3. EvalError
4. URIError
5. TypeError
6. RangeError
7. (generic) Error

NaN is NOT an error. 

A debugging workflow:
1. Look at the error message to find the relevant script that caused the problem
2. find the line number of the error
3. find the type of error
4. Check how far the script is running (use tools such as the console)
5. Use breakpoints where things are going wrong

***TRY, CATCH, FINALLY***  
Try, catch, finally - each one is given its own code block to tell the computer to 
1. try to execute the code **try**
2. if there's an exception, run *this* code **catch**
3. *always* run this code **finally**

Always remove your breakpoints/consolelogs/debuggers from live code!

<hr />

[Previous - Class 9 reading notes](class-09.md) 
[Next - Class 11 reading notes](class-11.md) 

[Return to Table of Contents](README.md)