# Unit Testing
- software testing technique where individual components are tested in isolation
	- *unit* is smallest testable part of application
		- like function, method, or class
## Key Principles of Unit Testing
- Isolation
	- each test focus on single unit of code and not depend on external systems/ other units
- Automation
	- tests run automatically
- Repeatability
	- tests produce same result every time they run
- Independence
	- tests don't depend on each other/ require specific execution order
- Fast Execution
	- tests run quickly to enable frequent testing
## Best Practices
- Write tests first
	- or alongside implementation
- Keep tests simple and focused
	- one logical concept per test
- Test behavior, not implementation
	- tests should survive refactoring
- Use meaningful assertions
	- include descriptive failure messages
- Avoid test interdependencies
	- each test should run independently
- Mock external dependencies
	- use mocking frameworks like Mockito
- Maintain tests like prod code
	- keep clean and refactored
- Run tests frequently
	- integrate with CI/CD pipelines
# Static Imports
- Static members in class can be independently imported in a static import
# Implementation
Start with defining constants
```java
private static final String EMPTY_LITERAL = "";
private static final String EMPTY_CONSTRUCTOR = new String();
private static final String FIVE_CHARACTERS = "ABCDE";
```
- Knowns that we can test on
Write testing methods
```java
@Test
public void emptyStringLengthTest() {
	assertAll("Tests for the empty string length() 0)",
		() -> assertEquals(0,
			EMPTY_LITERAL.length(),
				"The empty string literal should have a length of 0."),
		() -> assertEquals(0,
			EMPTY_CONSTRUCTOR.length(),
				"The empty string constructor should have a length of 0."),
	);
}

@Test
public void stringWithFiveCharactersTest() {
	final String name = "Jadon";
	assertAll("Tests for the empty string length() 5)",
		() -> assertEquals(5,
			FIVE_CHARACTERS.length(),
				"The string \"ABCDE\" should have a length of 5."),
		() -> assertEquals(5,
			EMPTY_CONSTRUCTOR.length(),
				"The string \"Jadon\" should have a length of 5."),
	);
}

@Test
public void stringEmptyStringisEmptyTest() {
	assertAll("Tests for the empty string isEmpty() true",
		() -> assertTrue(
			EMPTY_LITERAL.isEmpty(),
				"The empty string literal should return true on isEmpty()."),
		() -> assertTrue(
			EMPTY_CONSTRUCTOR.length(),
				"The empty string constructor should return true on isEmpty()."),
	);
}

@Test
public void stringNonEmptyStringisEmptyTest() {
	final String one = "1";
	assertAll("Tests for the non empty string isEmpty() false",
		() -> assertFalse(
			FIVE_CHARACTERS.isEmpty(),
				"The five character string literal should return false on
				 "isEmpty()."),
		() -> assertFalse(
			one.isEmpty(),
				"The non empty string of size 1 should return false on
				 "isEmpty()."),
	);
}
```
- Descriptive name
	- ends in Test
- Needs @Test assertation
- Parts of `assertEquals`
	- Expected value
	- Actual value
	- Error message
- `assertEquals` should not be done sequentially
	- if one fails, next will not run
- `assertAll` takes comma separated list of lambda expression tests
	- Runs all tests no matter if one fails
	- Should be used to group common tests
- `assertTrue` and `assertFalse` for Boolean values