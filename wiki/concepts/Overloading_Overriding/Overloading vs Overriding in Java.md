---
title: "Overloading vs Overriding in Java"
source: "https://www.geeksforgeeks.org/java/difference-between-method-overloading-and-method-overriding-in-java/"
author:
  - "[[GeeksforGeeks]]"
published: 2019-10-03
created: 2026-04-06
description: "Your All-in-One Learning Portal: GeeksforGeeks is a comprehensive educational platform that empowers learners across domains-spanning computer science and programming, school education, upskilling, commerce, software tools, competitive exams, and more."
tags:
  - "clippings"
---
Last Updated: 14 Oct, 2025

Method Overloading and Method Overriding allow methods with the same name but different behavior, supporting polymorphism, the ability of one name to represent multiple forms.

![[method_overloading_compile_time_polymorphism_.webp|method_overloading_compile_time_polymorphism_]]

[Method Overloading](https://www.geeksforgeeks.org/java/different-ways-method-overloading-java/) occurs when we have multiple methods in the same class with the same name but have different numbers of parameters. It allows performing operations with different inputs.

  
**Output**
```
my_Sum with 2 int parameters: 10
my_Sum with 3 int parameters: 17
```

****Explanation:**** The my\_Sum method is overridden in the child class. At runtime, Java determines which version to call based on the actual object. Calling my\_Sum(5, 10) on a Calculator object uses the parent class method, while calling it on an AdvancedCalculator object uses the overridden child class method. This demonstrates runtime (dynamic) polymorphism.

### Method Overriding (achieved at run time)

[Method Overriding](https://www.geeksforgeeks.org/java/overriding-in-java/) is redefining a superclass method in a subclass with the same signature and a compatible return type. It enables runtime polymorphism, where the JVM calls the method based on the actual object type.

  
**Output**
```
DerivedClass display() method
BaseClass show() method
```

****Explanation:**** Even though bs is a BaseClass reference, it actually points to a DerivedClass object. So, when we call display(), Java runs the DerivedClass version because it’s overridden. The show() method wasn’t changed in the subclass, so calling it just runs the BaseClass version.

The differences between Method Overloading and Method Overriding in Java are as follows:

| Feature | Method Overloading | Method Overriding |
| --- | --- | --- |
| ****Definition**** | Defining multiple methods with the same name but different parameters in the same class. | Redefining a parent class method in the subclass with the same signature and compatible return type. |
| ****Purpose**** | To achieve compile-time polymorphism (static binding). | To achieve runtime polymorphism (dynamic binding). |
| ****Parameter Lis**** t | Must be different (in number, type, or order). | Must be exactly the same as in the parent class. |
| ****Return Type**** | Can be same or different, but must not conflict. | Must be same or covariant (subtype of parent’s return type). |
| ****Inheritance**** | Not required; can occur within the same class. | Requires inheritance between superclass and subclass. |
| ****Access Modifier**** | Can have any access modifier. | Cannot reduce parent method’s access level. |
| ****Static / Final Methods**** | Can be overloaded. | Cannot be overridden if marked static or final. |
| ****Binding Time**** | Compile-time binding. | Runtime binding. |
| ****Exception Handling**** | Overloaded methods can declare any exceptions. | Overridden method cannot throw broader checked exceptions than the parent. |
| ****Example**** | void add(int a, int b) and void add(double a, double b) | Parent: void show() → Child: void show() |

[View All](https://www.geeksforgeeks.org/courses)

```
→
```

[View All](https://www.geeksforgeeks.org/jobs?tab_type=featured)

```
→
```