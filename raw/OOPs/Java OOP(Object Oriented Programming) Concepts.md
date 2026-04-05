---
title: "Java OOP(Object Oriented Programming) Concepts"
source: "https://www.geeksforgeeks.org/java/object-oriented-programming-oops-concept-in-java/"
author:
  - "[[GeeksforGeeks]]"
published: 2023-06-23
created: 2026-04-05
description: "Your All-in-One Learning Portal: GeeksforGeeks is a comprehensive educational platform that empowers learners across domains-spanning computer science and programming, school education, upskilling, commerce, software tools, competitive exams, and more."
tags:
  - "clippings"
---

Object-Oriented Programming (OOP) is a programming paradigm based on the concept of objects that contain data (fields) and behavior (methods). It focuses on designing software that closely represents real-world entities. It is used to:

- Improves code reusability
- Enhances maintainability and scalability
- Makes programs easier to understand and manage
- Closely models real-world entities

## Characteristics of an OOP(Object Oriented Programming)

The diagram below demonstrates the Java OOPs Concepts

![[Types-of-OOPS-2.gif|Types-of-OOPS-2]]

OOP's concept

### Class

A [Class](https://www.geeksforgeeks.org/java/classes-objects-java/) is auser-defined blueprint or prototype from which objects are created. It represents the set of properties or methods that are common to all objects of one type. Using classes, you can create multiple objects with the same behavior instead of writing their code multiple times. In general, class declarations can include these components in order:

- ****Modifiers****: A class can be public or have default access (Refer to [this](https://www.geeksforgeeks.org/java/access-modifiers-for-classes-or-interfaces-in-java/) for details).
- ****Class name:**** The class name should begin with the initial letter capitalized by convention.
- ****Body:**** The class body is surrounded by braces, { }.

****Example:**** A Car represents a class (blueprint), while BMW, Mercedes, and Audi represent objects (instances) created from that class.

![[Class.webp|Class]]

class-object

### Object

An [Object](https://www.geeksforgeeks.org/java/object-class-in-java/) is a basic unit of Object-Oriented Programming that represents real-life entities. A typical Java program creates many objects, which as you know, interact by invoking methods. The objects are what perform your code, they are the part of your code visible to the viewer/user. An object mainly consists of:

- ****State****: It is represented by the attributes of an object. It also reflects the properties of an object.
- ****Behavior****: It is represented by the methods of an object. It also reflects the response of an object to other objects.
- ****Identity****: It is a unique name given to an object that enables it to interact with other objects.
- [****Method****](https://www.geeksforgeeks.org/java/methods-in-java/)****:**** A method is a collection of statements that perform some specific task and return the result to the caller.

### Abstraction

[Abstraction in Java](https://www.geeksforgeeks.org/java/abstraction-in-java-2/) is the process of hiding implementation details and showing only the essential features of an object. It helps users focus on what an object does rather than how it does it.

- ****Hides complexity:**** Internal implementation details are hidden from the user.
- ****Improves maintainability:**** Changes in implementation do not affect the user code.
- ****Enhances flexibility:**** Supports loose coupling through abstract classes and interfaces.

****Example:**** An ATM or a coffee machine represents abstraction, where the user interacts with simple operations while the internal working and implementation details remain hidden.

![[hides_certain_details_and_show_only_essential_information.webp|hides_certain_details_and_show_only_essential_information]]

Abstraction

### How to Achieve Abstraction

- It is achieved in Java using [abstract classes](https://www.geeksforgeeks.org/java/abstract-classes-in-java/) and [interfaces](https://www.geeksforgeeks.org/java/interfaces-in-java/).
- [Interfaces](https://www.geeksforgeeks.org/java/interfaces-in-java/) can provide 100% abstraction, while abstract classes provide partial abstraction.
![[abstraction.webp|abstraction]]

### Encapsulation

[Encapsulation](https://www.geeksforgeeks.org/java/encapsulation-in-java/) is the process of wrapping data and methods into a single unit, usually a class, and restricting direct access to the data. It acts as a protective shield that prevents data from being accessed directly from outside the class.

- Data members are hidden using the private access modifier.
- Access to data is provided through public getter and setter methods.
- It improves data security, maintainability, and controlled access.
![[Encapsulation.webp|Encapsulation]]

Encapsulation

### Association

[Association](https://www.geeksforgeeks.org/java/association-composition-aggregation-java/) is an OOP concept that defines a relationship between two or more classes that are connected to each other. It represents how objects interact with each other and communicate. In association, objects of one class are related to objects of another class, but they can exist independently.

- Represents a relationship between objects
- Does not imply ownership
- Objects are independent of each other
- Helps in building flexible and modular systems
![[Associatn.png|Associatn]]

association

### Types of Association

Association in Java can be further classified into the following types:

### 1\. Aggregation (Weak Association)

Aggregation represents a “has-a” relationship where one class contains a reference to another class, but both can exist independently.

- It is a weak relationship
- Objects have independent lifecycles
- One object can exist without the other
- ****Example:**** A Department has Employees, but employees can exist even if the department is removed

### 2\. Composition (Strong Association)

[Composition](https://www.geeksforgeeks.org/java/composition-in-java/) is a strong form of association where one class owns another class. If the parent object is destroyed, the child object also gets destroyed.

- It is a strong relationship
- Objects have dependent lifecycles
- Child object cannot exist without the parent
- ****Example:**** A Car has an Engine

### Inheritance

[Inheritance](https://www.geeksforgeeks.org/java/inheritance-in-java/) is a core OOP concept in Java that allows one class to acquire the fields and methods of another class using the extends keyword. It represents an “is-a” relationship between classes.

- The class being inherited is called the superclass, and the inheriting class is the subclass.
- A subclass can use existing features of the superclass and also add its own.
- Inheritance promotes code reusability and reduces redundancy.

****Example****: Dog, Cat, Cow can be Derived Class of Animal Base Class.

![[inheritance-660x454.png|inheritance-660x454]]

Inheritance

### Types of Inheritance in Java

![[inheritance_in_java.webp|inheritance_in_java]]

Java supports the following types of inheritance:

- ****Single Inheritance:**** One subclass inherits from one superclass.
- ****Multilevel Inheritance:**** A class is derived from another derived class, forming a chain.
- ****Hierarchical Inheritance:**** Multiple subclasses inherit from a single superclass.
- ****Multiple Inheritance (through Interface):**** A class inherits from multiple interfaces since Java does not support multiple inheritance using classes.
- ****Hybrid Inheritance (through Interface):**** A combination of two or more types of inheritance, achievable using interfaces.

### Polymorphism

The word [****polymorphism****](https://www.geeksforgeeks.org/java/polymorphism-in-java/) means having ****many forms****, and it comes from the Greek words ****poly (many)**** and ****morph (forms)****, this means one entity can take many forms. In Java, polymorphism allows the same method or object to behave differently based on the context, specially on the project's actual runtime class.

![[polymorphism_in_java.webp|polymorphism_in_java]]

Polymorphism in Java

### Types of Polymorphism

Polymorphism in Java is mainly of 2 types as mentioned below:

****1\. Compile-time Polymorphism(****[Method Overloading](https://www.geeksforgeeks.org/java/method-overloading-in-java/)****):****Achieved when multiple methods have the same name but different parameters. The method call is resolved at compile time.

****2\. Runtime Polymorphism (****[Method Overriding](https://www.geeksforgeeks.org/java/overriding-in-java/) ****):**** Achieved when a subclass provides a specific implementation of a method already defined in its superclass. The method call is resolved at runtime based on the object

### Advantage of OOP over Procedure-Oriented Programming Language

Object-oriented programming (OOP) offers several key advantages over procedural programming:

- ****Code reusability:**** Classes and objects allow reuse of existing code, reducing duplication and improving efficiency.
- ****Better structure and maintainability:**** Programs are organized into logical units, making code easier to understand, debug, and maintain.
- ****Supports DRY principle:**** Common functionality is written once and reused, leading to cleaner and more maintainable code.
- ****Faster development:**** Modular and reusable components help in quicker and scalable application development.

### Disadvantages of OOP

- ****Steep learning curve:**** Concepts like classes, objects, inheritance, and polymorphism can be difficult for beginners.
- ****Overhead for small programs:**** OOP may require more code and structure than necessary for simple applications.
- ****Debugging complexity:**** Code spread across multiple classes and layers can make debugging more time-consuming.
- ****Higher memory usage:**** Creating many objects can consume more memory compared to procedural programs.

3 Questions

![[sucess-img.png|success]]

Quiz Completed Successfully

Your Score:0/3

Accuracy:0%

Article Tags:

[Java](https://www.geeksforgeeks.org/category/programming-language/java/)

[View All](https://www.geeksforgeeks.org/courses)

```
→
```

[View All](https://www.geeksforgeeks.org/jobs?tab_type=featured)

```
→
```