# Observer Design Pattern
## Problem
- We might have a mutable state that is implemented in some part of application. 3rd parties interested in that state
	- Traditionally state would have reference to each 3rd party
 ```java
class state {
	setLocation() {
		myA.changeLocation();
		myB.setLocation();
		myC.checkLocation();  
	}
}
```
- Changing functionality requires editing state class 
## Pattern
- State is called *Model*
- Interested parties are *Views*
- At runtime views can be added and removed
- Model calls updates for all current views
- Almost always uses an Observer interface
	- Has update method 
	- Views implement observer
- 