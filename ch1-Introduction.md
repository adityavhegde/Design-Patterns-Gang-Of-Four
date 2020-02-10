## History 

The book was written back in 1994. This is the first book to have named these patterns. At the time the book was written Java was an emerging languaged and C++ and Smalltalk were the popular language. The book makes references to Smalltalk. What I understand about these references is that Smalltalk is a pure OO language.

Smalltalk as a language is kind of 3 things, partly an Operating System of its own. In a sense this reminds me of Erlang VM. Objects in Smalltalk don't have a type and in the sense of Pure OO -- the Objects message and talk to each other. This is not different from the Actor model [2].

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

## OO Concepts 

The main highlights here are 

1. Programing to an Interface and not an Implementation
2. Favor Object composition over inheritance 
3. Don't overdo it, but wherever possible use delegation to overcome problems with composition
4. Use a balance of both approaches 

**Programming to an interface** 
1. Clients don't need to know class type and underlying implementation -- just know the interface 
2. If clients only use the interface, you can change the underlying implementation any time you want, so long as you stick to the interface. 

Inheritance: simple to follow because this happens at compile time. However child sublcasses are tied to parent class. Re-write to parent class breaks child functionalities. **Overcome this by subclassing from Abstract classes**

**Delegation**
Hold a reference to composed object and allow the composed object to implement functionality.
Cons: harder to debug and reason about.

**Run Time and Compile Time structures**
A programs compile time structure is the class and the run time aspect is the object and therefore we should think about them differently as they are independent structures.

The run time interactions are more dictated by the Architect.

Throw in mentions of Aggregation and Aquaintance. 

## Design aspects to keep in mind 

1. Don't create an object by using specific class: rather use an Interface 
2. Avoid tightly coupled classes 
3. Hardware dependent implementations should be avoided to favour platform independence 

Choice in design pattern applicability depends on your area:
1. Is this an Application Program
2. Is this a toolkit 
3. Or it this a framework 

Frameworks: takes mental load off boilerplate.

## Questions 
1. Is try-catch in Java Chain of Responsibility pattern 
2. Memory Overhead of classes and garbage collection strategies 
3. Jax RS ? 
4. How can you use objects to handle code pre-conditions and error handling

## References 
1. Design Patterns - Elements of Reusable Object Oriented Software
2. https://stackoverflow.com/questions/58578030/what-is-the-difference-between-processes-messages-in-erlang-and-objects-messages

## Authors 
Aditya Hegde

