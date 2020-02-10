## History 

The book was written back in 1994. This is the first book to have named these patterns. At the time the book was written Java was an emerging languaged and C++ and Smalltalk were the popular language. The book makes references to Smalltalk. What I understand about these references is that Smalltalk is a pure OO language.

Smalltalk as a language is kind of 3 things, partly an Operating System of its own. In a sense this reminds me of Erlang VM. Objects in Smalltalk don't have a type and in the sense of Pure OO -- the Objects message and talk to each other. This is not different from the Actor model.

Talking about objects as if they are operating system processes. It is important to note that these are programming abstractions, meaning your object is either in the executing stack or page of memory on the heap which is used by the current running process. Even though the authors talk about objects like some sort of process and inter process communication, it's just a programming abstraction and not an operating system construct. Everything finally runs as a process or a group of processes or threads within a process. It is also mentioned at some point that OO in itself is a **design pattern**.

Two key reasons to use OO:
1. Code re-use via inheritance 
2. Encaspsulating mutable state 

It is no surprise that early GUI application is where OO actually emerged. 

### Side Note: from a web context 

Web based applications can greatly be simplified by identifying entities in your database and then representing them via Model classes. Essentially this could be your objects in the system. It helps reason about the code well and provide simpler user interfaces. 

## Smalltalk MVC 
Nothing new here. The order in which M or V or C come are slightly different compared to a web application using MVC. 

View references Controller to implement a response strategy. 

Models represent data/database and can also contain business logic (depending on what pattern you like -- fat models v/s thing models) 

MVC feature: Views can be nested into a Composite View.

## Organization of patterns 

1. Structural 
2. Creational 
3. Behavioral 

Their scopes could be the class or the object. 

**Class patterns** 

deal with relationships between classes

compile time

**Object patterns** 

deal with object relationships 

dynamic -- change at runtime 



## References 
1. Design Patterns - Elements of Reusable Object Oriented Software 

## Authors 
Aditya Hegde

