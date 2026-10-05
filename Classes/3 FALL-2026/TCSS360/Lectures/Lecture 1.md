# Class Diagram
- Every class has name
- Classes can have attributes and methods
	- Visibility
- Classes can have different relationships between them
	- Extend

# Object Oriented Principles
- Encapsulate what varies
	- Provide only necessary information to other classes
	- One class should only do one thing
	- All methods using data that we know will change should not be in class with static data
- Favor composition over inheritance
	- Lots of inheritance leads to high coupling
		- Needing to modify one thing then creates a lot of work
	- Composition: B only exists if A exists
- Program to an interface, not an implementation
	- Program at higher level of abstraction
- Strive for loosely coupled designs between objects that interact
- Classes should be open for extensions but closed for modification
- Depend on abstraction, not concrete class
	- Use interfaces and abstract classes, rather than actual implementation
- Only talk to your friends
	- Classes only communicate with classes they extend
	- Don't call nested classes
-  Don't call us, we'll call you
	- Wait for input to run certain code
- Class should only have one reason to change
	- Single responsibility
# Object Oriented Basics
- Abstraction
- Encapsulation
- Polymorphism
- Inheritance
# SOLID
- Single Responsibility Principle
- Open-closed principle
	- extend rather than modify
- Liskov substitution principle
	- Related to polymorphism but more strict
- Interface segregation principle
	- clients should not depend of interface methods they do not use
- Dependency inversion principle
	- Depend on abstraction rather than concrete