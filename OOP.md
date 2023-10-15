#OOP
Object Oriented Programming (also known as OOPs) is a programming paradigm where the complete software operates as a bunch of objects talking to each other. An object is a collection of data and the methods which operate on that data.
What is a Class?
A class is a building block of Object Oriented Programs. It is a user-defined data type that contains the data members and member functions that operate on the data members. It is like a blueprint or template of objects having common properties and methods.

4. What is an Object?
An object is an instance of a class. Data members and methods of a class cannot be used directly. We need to create an object (or instance) of the class to use them. In simple terms, they are the actual world entities that have a state and behavior.

The main feature of the OOPs, also known as 4 pillars or basic principles of OOPs are as follows:

Encapsulation
Data Abstraction
Polymorphism
Inheritance

#### <ins> <b>Polymorphism:</b>
In the object-oriented programming paradigm, Polymorphism is the ability of an action or method to perform different functions based on the object it’s acting upon. Some aspects of Polymorphism include overloading, overriding and dynamic method binding.
Polymorphism can be classified into two types based on the time when the call to the object or function is resolved. They are as follows:

A. Compile Time Polymorphism
B. Runtime Polymorphism

A) Compile-Time Polymorphism

Compile time polymorphism, also known as static polymorphism or early binding is the type of polymorphism where the binding of the call to its code is done at the compile time. Method overloading or operator overloading are examples of compile-time polymorphism.

B) Runtime Polymorphism

Also known as dynamic polymorphism or late binding, runtime polymorphism is the type of polymorphism where the actual implementation of the function is determined during the runtime or execution. Method overriding is an example of this method.
<li><b>What is static polymorphism? </b>Static polymorphism (static binding) is a kind of polymorphism that occurs at compile time. An example of compile-time polymorphism is method overloading.</li>
 <li><b>What is dynamic polymorphism? </b>Runtime polymorphism or dynamic polymorphism (dynamic binding) is a type of polymorphism which is resolved during runtime. An example of runtime polymorphism is method overriding.</li>
 <li><b>What is method overloading?</b> Method overloading is a feature of OOPs which makes it possible to give the same name to more than one methods within a class if the arguments passed differ.</li>
 <li><b>What is method overriding?</b>Method overriding is a feature of OOPs by which the child class or the subclass can redefine methods present in the base class or parent class. Here, the method that is overridden has the same name as well as the signature meaning the arguments passed and the return type.</li>
 <li><b>What is operator overloading?</b>Operator overloading refers to implementing operators using user-defined types based on the arguments passed along with it.</li><br>
-----------------------------
<li><b>What does SOLID mean? What are its principles?</b>

<ul><li><b>S -</b> Single-responsibility principle. A class should have only one job</li>
<li><b>O - </b>Open-closed principle. Objects must be open for extension but closed for modification.</li>
<li><b>L - </b>Liskov substitution principle. Let q (x) be a property provable about objects of x of type T. Then q (y) should be provable for objects y of type S where S is a subtype of T.</li>
<li><b>I - </b>Interface segregation principle. You cannot force clients to implement an interface that they are not using.</li>
<li><b>D - </b>Dependency Inversion Principle. Entities must depend on abstractions, not on concretions.</li></ul>
</li>
<li><b>class: </b> class is a prototype that consists of objects in different states and with different behaviors. It has a number of methods that are common the objects present within that class.</li>
<li><b>Structure: </b>A structure is basically a user-defined collection of variables which are of different data types.</li>

#### <ins> Inheritance
 Inheritance is a feature of OOPs which allows classes inherit common properties from other classes. For example, if there is a class such as ‘vehicle’, other classes like ‘car’, ‘bike’, etc can inherit common properties from the vehicle class. This property helps you get rid of redundant code thereby reducing the overall size of the code. There are 5 types: Single inheritance, Multiple inheritance, Multilevel inheritance,Hierarchical inheritance, and Hybrid inheritance.
<li><b>Multiple Inheritance: </b>Multiple inheritance comes into picture when a class inherits more than one base class</li>
<li><b>Multilevel inheritance</b> means a class inherits from another class which itself is a subclass of some other base class</li>
 <li><b>Hybrid inheritance</b> is a combination of multiple and multi-level inheritance.</li>
 <li><b>Hierarchical inheritance</b> refers to inheritance where one base class has more than one subclasses. For example, the vehicle class can have ‘car’, ‘bike’, etc as its subclasses.</li>

 ###### <b>Limitations of Inheritance</b>
 <li>Increases the time and effort required to execute a program as it requires jumping back and forth between different classes</li>
 <li>The parent class and the child class get tightly coupled</li>
 <li>Any modifications to the program would require changes both in the parent as well as the child class</li>
<li>Needs careful implementation else would lead to incorrect results</li>
------------------------------

 <li><b>Encapsulation: </b>refers to binding the data and the code that works on that together in a single unit. For example, a class. Encapsulation also allows data-hiding as the data specified in one class is hidden from other classes.</li>
 <li><b>Access specifiers: </b>Access specifiers or access modifiers are keywords that determine the accessibility of methods, classes, etc in OOPs. These access specifiers allow the implementation of encapsulation. The most common access specifiers are public, private and protected. However, there are a few more which are specific to the programming languages.</li>

 Encapsulation is the binding of data and methods that manipulate them into a single unit such that the sensitive data is hidden from the users
It is implemented as the processes mentioned below:

Data hiding: A language feature to restrict access to members of an object. For example, private and protected members in C++.
Bundling of data and methods together: Data and methods that operate on that data are bundled together. For example, the data members and member methods that operate on them are wrapped into a single unit known as a class.

------------------------------

 #### <ins> Data abstraction
Abstraction is similar to data encapsulation and is very important in OOP. It means showing only the necessary information and hiding the other irrelevant information from the user. Abstraction is implemented using classes and interfaces.
 <li><b>abstract class </b>An abstract class is a class that consists of abstract methods. These methods are basically declared but not defined. If these methods are to be used in some subclass, they need to be exclusively defined in the subclass.</li>
 <li><b>Can you create an instance of an abstract class? </b>No. Instances of an abstract class cannot be created because it does not have a complete implementation. However, instances of subclass inheriting the abstract class can be created.</li>
 <li><b>What is an interface? </b>It is a concept of OOPs that allows you to declare methods without defining them. Interfaces, unlike classes, are not blueprints because they do not contain detailed instructions or actions to be performed. Any class that implements an interface defines the methods of the interface.</li>
------------------------------ <br>
<br>
<li><b>Differentiate between a class and a method</b></li>
<img src=./class-method.png></img>

--------------------

### <ins>  paradigms of programming exist besides OOPs
The programming paradigm is referred to the technique or approach of writing a program. The programming paradigms can be classified into the following types:
1. Imperative Programming Paradigm
It is a programming paradigm that works by changing the program state through assignment statements. The main focus in this paradigm is on how to achieve the goal. The following programming paradigms come under this category:

Procedural Programming Paradigm: This programming paradigm is based on the procedure call concept. Procedures, also known as routines or functions are the basic building blocks of a program in this paradigm.
Object-Oriented Programming or OOP: In this paradigm, we visualize every entity as an object and try to structure the program based on the state and behavior of that object.
Parallel Programming: The parallel programming paradigm is the processing of instructions by dividing them into multiple smaller parts and executing them concurrently.
2. Declarative Programming Paradigm
Declarative programming focuses on what is to be executed rather than how it should be executed. In this paradigm, we express the logic of a computation without considering its control flow. The declarative paradigm can be further classified into:

Logical Programming Paradigm: It is based on formal logic where the program statements express the facts and rules about the problem in the logical form.
Functional Programming Paradigm: Programs are created by applying and composing functions in this paradigm.
Database Programming Paradigm: To manage data and information organized as fields, records, and files, database programming models are utilized.

-------
What is Constructor?
A constructor is a block of code that initializes the newly created object. A constructor resembles an instance method but it’s not a method as it doesn’t have a return type. It generally is the method having the same name as the class but in some languages, it might differ. 


What is a ternary operator?
The ternary operator is said to be an operator which takes three arguments. Arguments and results are of different data types, and it depends on the function. The ternary operator is also called a conditional operator.

What is ‘this’ pointer?
THIS pointer refers to the current object of a class. THIS keyword is used as a pointer which differentiates between the current object with the global object. It refers to the current object.
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
<li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
<li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
<li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
<li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>

