# Utility Class
- Class never intended to be instantiated
	- No public constructor
- Static methods in utility classes
- Ex) 
  ```
  Math.pow()
  ```
  - Never instantiated, `pow()` is a static method
  - `final` keyword prevents class from having children
# Static Initialization Block
```
static {

}
```
- Can have as many as you want
- Always executed only once when class is first touched
- Used for initializing static members before constructors