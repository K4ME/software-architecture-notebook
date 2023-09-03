Source [c4model](https://c4model.com/)

# Maps of your code

The C4 model was created as a way to help software development teams describe and communicate software architecture

![image](https://github.com/K4ME/software-architecture-notebook/assets/33429566/67cdd5be-927a-4c16-9c09-f8a4aaf2b454)


The C4 model is an "abstraction-first" approach to diagramming software architecture, based upon abstractions that reflect how software architects 
and developers think about and build software. The small set of abstractions and diagram types makes the C4 model easy to learn and use. 

![image](https://github.com/K4ME/software-architecture-notebook/assets/33429566/55d29f0c-16ec-4dcf-9400-fce6da5282a0)

# Abstractions

In order to create these maps of your code, we first need a common set of abstractions to create a ubiquitous language that we can use to describe the static structure of a software system. A software system is made up of one or more containers (applications and data stores), each of which contains one or more components, which in turn are implemented by one or more code elements (classes, interfaces, objects, functions, etc). And people may use the software systems that we build.

![image](https://github.com/K4ME/software-architecture-notebook/assets/33429566/2e0ad024-c9f1-42e3-9164-eb33e78e047c)


# System Context diagram

A System Context diagram is a good starting point for diagramming and documenting a software system, allowing you to step back and see the big picture. 
Detail isn't important
The focus should be on people (actors, roles, personas, etc) and software systems rather than technologies, protocols and other low-level details.

![image](https://github.com/K4ME/software-architecture-notebook/assets/33429566/15da58e4-0862-48fa-be28-d838bfd2bad0)


# Container diagram

Essentially, a container is a separately runnable/deployable unit that executes code or stores data.
A "container" is something like a server-side web application, single-page application, desktop application, mobile app, database schema, file system, etc. 

![image](https://github.com/K4ME/software-architecture-notebook/assets/33429566/71923a31-0c7f-432e-b679-f4b787da2d37)



# Component diagram

The Component diagram shows how a container is made up of a number of "components", what each of those components are, their responsibilities and the technology/implementation details.

![image](https://github.com/K4ME/software-architecture-notebook/assets/33429566/68d9d6ee-7c06-4cc0-865d-5ae18b9ce653)


# Code diagram

This is an optional level of detail and is often available on-demand from tooling such as IDEs.
You can zoom in to each component to show how it is implemented as code; using UML class diagrams, entity relationship diagrams or similar.

![image](https://github.com/K4ME/software-architecture-notebook/assets/33429566/b3f80a6e-fcd9-439c-9fd5-ae02e4ebfff1)
