
# Design Patterns 

- [Design Patterns](#design-patterns)
  - [Why do we need Design patterns](#why-do-we-need-design-patterns)
- [Design Principles that facilitate Change in a software system.](#design-principles-that-facilitate-change-in-a-software-system)
  - [Design pattern categories](#design-pattern-categories)
  - [Observer pattern](#observer-pattern)

## Why do we need Design patterns

Design patterns exist to make our code friendly to the one constant in software; change. Design patterns provide us with a **general reusable solution** to encapsulate what changes from what stays the same. Design patterns are programming language independent strategies. That means a design pattern represents an idea, not a particular implementation. 

Last but not least, design patterns are about establishing vocabularies for communicating solutions to other developers.


# Design Principles that facilitate Change in a software system.

- Favor composition to inheritance.
- 


## Design pattern categories

Design patterns are divided in to 3 major categories

 - Creational Pattern :

    Creational patterns are focused on **automatic object creation** instead of manual instantiation. Creational patterns take advantage of **polymorphism**. Creational patterns take control of our object creation. Consider it autopilot for object creation.

    Creational patterns help us achieve open/closed principle.

 - Structural Pattern :
  
    Structural pattern is about how larger structures are built from individual parts, generally of different classes. Structural patterns take advantage of **interfaces** and **inheritance** 
    
    vary a great deal depending on what sort of structure is being created for **what purpose**.


 - Behavioral Pattern :
  
   This type of patterns describe **interactions** between objects and focus on how objects **communicate** with each other. These patterns describe not just  patterns of objects or classes but also the **patterns of communication** between them. 

   Behavioral patterns shift your focus away from the flow of control to let you concentrate just on the way objects are interconnected. **Behavioral class patterns use inheritance to distribute behavior between classes**.


## Observer pattern

observer design pattern is a behavioral design pattern that lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they are observing.

