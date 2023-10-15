<ul>
<li><b>What is the difference between == and ===?:&nbsp;</b>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;== checks for value equality, while === checks for both value and type equality.</li>
<li><b>What is the difference between an anonymous function and a named function?</b>A named function can be referenced in the future from anywhere in the code, whereas an anonymous function cannot — although it will run when it occurs in-line.</li>
<li><b>What is an event loop?</b></li>
<li><b>null vs undefined values: </b>
<ul><li><b>Undefined:</b> Undefined is a built-in value in JavaScript that indicates the absence of a value. It is typically assigned automatically to a variable that has been declared but has not been assigned a value. Undefined is also returned when accessing a non-existent property on an object or when a function does not explicitly return a value.</li>
<code>let myVariable; // undefined</code> => myVariable is declared but not assigned a value, so its initial value is undefined.
<li><b>Null:</b> Null is also a built-in value in JavaScript, but it represents the intentional absence of any object value. It is explicitly assigned to a variable to indicate that it has no value or that an object reference is intentionally empty. Unlike undefined, null is a value that you can assign to a variable explicitly to indicate the absence of an object or a known empty value. </li>
<code>let myVariable = null;</code> => myVariable is declared but not assigned a value, so its initial value is undefined.
 <li><b>Distinguishing Factors:</b></li>
 <b>Automatic Assignment:</b>
 Undefined is automatically assigned to a variable that has been declared but not assigned a value. Null requires explicit assignment to indicate the absence of a value.<br>
<b>Type:</b>
 Undefined is a type of its own called “undefined.” Null is an object type.<br>
<b>Usage:</b>
 Undefined is commonly used to represent the absence of a value or when an expected value is missing. Null is typically used to indicate that a variable intentionally has no value or an object reference is intentionally empty.
 
</ul>
</li>

 <li><b>prototypal inheritance: </b>JavaScript uses prototypal inheritance as its primary mechanism for object-oriented programming. Prototypal inheritance allows objects to inherit properties and methods from other objects, known as prototypes.</li>
 <li><b>Coercion: </b>Coercion is a JavaScript conversion between two different built-in types. There are two forms of coercion: explicit and implicit.

Here is an example of explicit coercion:

```JS
var a = "42";
var b = Number (a)
a; // "42" - the string
b; // 42 - the number!
```

Here's an example of an implicit coercion:

```JS
var a = "42";
var b = a * 1; // "42" implicitly coerced to 42 here
a; // "42"
b; // 42 - the number!
```
</li>
 <li><b>Callback functions: </b> Callback functions are a key part of JavaScript. Callbacks are used to develop asynchronous code by ensuring a given function is not going to run until after a given task is completed. Callback functions take advantage of the fact that functions themselves are objects and may be passed as arguments to another function. </li>
 <li><b>Lexical Scoping: </b>The visibility and access of variables and functions is affected by the scope in which they are declared. These items can be global in scope, and therefore accessible to all code, or local to a block of code or function. Inner functions are lexically bound by outer functions, meaning they have access to variables declared by their outer functions.</li>
 <li><b>What and how to use a Class: </b> A class is essentially a template for encapsulated, reusable code for which there may be multiple instances of (referred to as objects), as you would in any object oriented language. Classes contain data in the form of variables and functions that execute code. You declare classes either as functions or with the class keyword. Classes have a special function called a constructor used to set its internal values when a new instance is created. Other functions may be called on an instance as needed.
 
 ```JS
 class Employee {
  constructor(name_param) {
    this.name = name_param;
  }
}
var employeeInstance1 = new Employee("Brianna");
var employeeInstance2 = new Employee("Sophia");
console.log(employeeInstance1.name); // prints "Brianna" to the console
console.log(employeeInstance2.name); // prints "Sophia" to the console
 ```
 </li>
<li><b>How to handle asynchronous calls: </b> Callbacks & Promises</li>
<li><b>Promise: </b>A Promise is a proxy for a value not necessarily known when the promise is created. It allows you to associate handlers with an asynchronous action's eventual success value or failure reason. This lets asynchronous methods return values like synchronous methods: instead of immediately returning the final value, the asynchronous method returns a promise to supply the value at some point in the future.</li>
<li><b>Ways to handle a promise: </b> Async/await is a different API to use promises. Async/Await provide a much nicer syntax in more complex scenarios. In particular, anything dealing with loops or certain other constructs like try/catch</li>
<li><b></b></li>
<li><b></b></li>
<li><b></b></li>
</ul>