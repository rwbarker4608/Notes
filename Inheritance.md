# Inheritance 

-   **Inheritance is a mechanism for deriving a new class from another class (base class).** 
-   The new class acquires some fields and methods of the base class. 
-   Inheritance is one of the main principles of object-oriented programming. It allows developers to build convenient class hierarchies and reuse existing code.

## Extending classes
When it comes to inheritance, there are several terms. A class derived from another class is called a subclass (it's also known as a derived class, extended class 
or child class). The class from which the subclass is derived is called a superclass (also a base class or a parent class).

To derive a new class from another the keyword extends is used. The common syntax is shown below.
class SuperClass { }

```javascript
class SubClassA extends SuperClass { }

class SubClassB extends SuperClass { }

class SubClassC extends SubClassA { }
```
There are important points about inheritance in Java:

-   Java doesn't support multiple-class inheritance meaning that a class can only inherit from a single superclass;
-   a class hierarchy can have multiple levels (class C can extend class B that extends class A);
-   a superclass can have more than one subclass.

A subclass inherits all public and protected fields and methods from the superclass. A subclass can also add new fields and methods.
A subclass doesn't inherit private fields and methods from the superclass. However, if the superclass has public or protected methods for accessing its private fields, 
these members can be used inside subclasses.

Constructors are not inherited, but the superclass's constructor can be invoked from the subclass using the special keyword super. 
