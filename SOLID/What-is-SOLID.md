SOLID is an acronym that stands for five key design principles: 
- [Single Responsibility Principle](#single-responsibility-principle)
- [Open-closed Principle](#open-closed-principle)
- [Liskov Substitution Principle](#liskov-substitution-principle)
- [Interface Segregation Principle](#interface-segregation-principle)
- [Dependency Inversion Principle](#dependency-inversion-principle)

The SOLID principles were developed by Robert C. Martin in a 2000 essay, [Design Principles and Design Patterns.](https://web.archive.org/web/20150906155800/http:/www.objectmentor.com/resources/articles/Principles_and_Patterns.pdf")

The broad goal of the SOLID principles is to reduce dependencies so that engineers change one area of software without impacting others. 
Additionally, they’re intended to make designs easier to understand, maintain, and extend. 
Ultimately, using these design principles makes it easier for software engineers to avoid issues and to build adaptive, effective, and agile software.

<br/>

<a id="single-responsibility-principle"></a>
###  Single Responsibility Principle (SRP) 

> "A class should have one, and only one, reason to change."
> Robert C. Martin

Which means, that each class only does one thing and every class or module only has responsability for one part of the software's functionality. 
**More simply, each class should solve only one problem.**

**This principle can be applied to classes, software components and microservices.**

<br/>

<a id="open-closed-principle"></a>
###  Open-closed Principle (OCP)

> "You should be able to extend a class's behavior without modifying it."
> Robert C. Martin

Following this principle is essential for writing code that is easy to maintain and revise.
Your class complies with this principle if it is:
- Open for extesion, meaning that the class's behavior can be extended.
- Closed for modification, meaning that the source code is set and cannot be changed.

<br/>

<a id="liskov-substitution-principle"></a>
### Liskov Substitution Principle (LSP)

The principle is named for Barbara Liskov, who introduced this concept of behavioral subtyping in 1987.

> "What is wanted here is something like the following substitution property: if for each object O1 of type S there id an object O2 of type T such that for all programs P defined in terms od T, the behavior of P is unchanged when O1 is substituted for O2 then S is a subtype of T."
> Barbara Liskov

**Simplifying,  Derived classes should be substitutable for their base classes. That is, a user of a base class should continue to function properly if a derivative of that base class is passed to it.**


<br/>

<a id="#interface-segregation-principle"></a>
### Interface Segregation Principle (ISP)

It's better to have a lot of smaller interfaces than a few bigger ones.

> "Make fine grained interfaces that are client-specific. Clients should not be forced to implement interfaces they do not use."
> Robert C. Martin

<br/>

<a id="#dependency-inversion-principle"></a>
### Dependency Inversion Principle (DIP)

This principle offers a way to decouple software modules, which means that developers should depend on abstractions, not on concretions.

High-level modules, which provide complex logic, should be easily reusable and unaffected by changes in low-level modules, which provide utility features. 
To achieve that, you need to introduce an abstraction that decouples the high-level and low-level modules from each other.

> "High level modules should not depend upon low level modules. Both should  depend on abstractions."
> Robert C. Martin
