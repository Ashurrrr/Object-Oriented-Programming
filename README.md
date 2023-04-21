# Object-Oriented-Programming

What's an object? In CS and object can be a variable, a data structure, a function or a method; therefore, a location in memory having a value that can be referenced by an identifier. In object oriented programming an onject is an instance of a class where this object can be either a variable, a function, a data structure or a combination of such. OOP designs programs with creation of objects an approach that focuses on the defintion of data rather than the input - processing - output logic (object oriented vs procedure-oriented). The goal is to create an object that we can define and provide functionality to solve problems. Using a dog as an example object, the dog may have attributes such as name, colour, breed, isHungry, isThirsty alongside methods like bark(), eat(), sleep().


A class is an abstract description of all objects that can be made from this set class where an object can be instantiated from. A class contains attributes that could be fields (variables that belong to an object or a class) or methods (funcrions that the object can call). The initialization method is executed as soon as an object of the class is instantiated. Self parameter is used to denote that the method is applied and accessible for the object itself. 


Encapsulation (information hiding) is restricting the access to the classes/objects certain attributes and methods. In python we hide attributes and methods by using a double underscore __ as a prefix.
Overloading is when two methods in one class have the same method name, but different parameters.
Overriding is when two methods have the same method name and parameters.
Polymorphism is a method that can be used across different classes and object that is dependant on the parameters.


Inheritance occurs when an onject or class is based on another class; where its feature are from a parent class
There are three different types: Single inheritance (A subclass inheriting the features of a single superclass / parent class), Multiple inheritance (A subclass inheriting the features of a multiple parent classes), and lastly Multilevel inheritance (A  subclass is inheriting from another subclass… A → B → C)
We can do many things with inheritance, for example, a child will receive all attributes and methods of the parent, the child can then enhance itself with new attributes and methods eventually overriding attributes and methods for their own liking/speciality.
super() is a bult in method for classes to refer their parent class.
