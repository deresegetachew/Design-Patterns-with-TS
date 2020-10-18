
# Design Patterns 

- [Design Patterns](#design-patterns)
  - [Why do we need Design patterns](#why-do-we-need-design-patterns)
- [Relationships between Objects](#relationships-between-objects)
- [Design Principles that facilitate Change in a software system.](#design-principles-that-facilitate-change-in-a-software-system)
  - [Design pattern categories](#design-pattern-categories)

## Why do we need Design patterns

Design patterns exist to make our code friendly to the one constant in software; change. Design patterns provide us with a **general reusable solution** to encapsulate what changes from what stays the same. Design patterns are programming language independent strategies. That means a design pattern represents an idea, not a particular implementation. 

Last but not least, design patterns are about establishing vocabularies for communicating solutions with other developers. design patterns allow a team to communicate in a functioning manner and reduce confusion. 


# Relationships between Objects

- Dependency:
  - most basic and weakest relationship between **classes**. it occurs when we use concrete class names in our code. e.g. specifying types in method signature.
  
- Association :
  - Association can be seen as a specialized kind of dependency, where an object always
    has access to the objects with which it interacts
  - Establishes a permanent link **between objects**
  - A field in a class or a method that returns object instances is an association
  
  - There are 2 types of Associations:
    - Aggregations : where the component the container depends on **can exist** with out the container.
     - Composition:  Where the componenet the container depends on **can not exist** with out the container

```typescript
  class Order {
    customer: Customer;
    lineItem: [orderLineItem]

    getShipmentInfo(){
      .....
     customer.getShipmentDetail()
      ....
    }
  }


class OrderLineItem {
  id: number,
  productId: number,

  getLineItem(product)
}
```
  In the example above Customer and Product are Associations with Order while Tax is a dependency. fields customer and lineItem are always accessible to any method of Order class thus not only is it depending on Customer class but it is also associated with it.

# Design Principles that facilitate Change in a software system.

- Encapsulate what changes
- Favor composition over inheritance.
- Program to Interfaces not to implementations (Depend on abstractions, not on concrete classes)
  - inheritance represents the **“is a” **relationship between
classes (a car is a transport), composition represents the **“has
a”** relationship (a car has an engine).
  - Aggregation is a relaxed variation of composition a more relaxed variant of composition where one object may have a reference to the other one but doesn’t manage its lifecycle. Here’s an example: a car has a driver, but he or she may use another car or just walk without the car.
- Strive for loosely coupled design between objects that interact (e.g. observer pattern)



## Design pattern categories

Design patterns are divided in to 3 major categories

 - Creational Pattern :

    Creational patterns are focused on **automatic object creation** instead of manual instantiation. Creational patterns take advantage of **polymorphism**. Creational patterns take control of our object creation. Consider it autopilot for object creation.
    
    Creational patterns help us achieve open/closed principle.
    The following are creational patterns I have covered here :

    - [Factory method](src/factory/readme.md)
    - [Abstract Factory](src/abstractFactory/readme.md)
    - [Builder](src/builder/readme.md)
    - [Prototype](src/prototype/readme.md)
    - [Singelton](src/signelton/readme.md)

 - Structural Pattern :
  
    Structural pattern is about how larger structures are built from individual parts, generally of different classes. Structural patterns take advantage of **interfaces** and **inheritance** 
    
    The following are structural patterns covered here:
  
   - [Adapter](src/adapter/readme.md)
   - [Bridge](src/bridge/readme.md)
   - [Composite](src/composite/readme.md)
   - [Decorator](src/decorator/readme.md)
   - [Facade](src/facade/readme.md)
   - [FlyWieght](src/flyweight/readme.md)
   - [Proxy](src/proxy/readme.md)


 - Behavioral Pattern :
  
   This type of patterns describe **interactions** between objects and focus on how objects **communicate** with each other. These patterns describe not just  patterns of objects or classes but also the **patterns of communication** between them. 

   Behavioral patterns shift your focus away from the flow of control to let you concentrate just on the way objects are interconnected. **Behavioral class patterns use inheritance to distribute behavior between classes**.


   The following are Behavioral design patterns

   - [Chain of Responsibility](src/chainOfResponsibility/readme.md)
   - [Command](src/command/readme.md)
   - [Iterator](src/iterator/readme.md)
   - [Mediator](src/mediator/readme.md)
   - [Memento](src/memento/readme.md)
   - [Observer](src/observer/readme.md)
   - [State](src/state/readme.md)
   - [Strategy](src/strategy/readme.md)
   - [Template Method](src/templateMethod/readme.md)
   - [Visitor](src/visitor/readme.md)

