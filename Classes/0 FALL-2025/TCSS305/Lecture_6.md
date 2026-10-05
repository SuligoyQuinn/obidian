  `String.charAt()` testing
```java
@test
public void charAtFiveCharStringTest() {
	final String fiveChars = "abcde";
	  
	assertAll("Testing charAt on \"abcde\" should return chars."
		() -> assertEquals('a', fiveChars.charAt(0),
		"Index 0 should be a"),
		() -> assertEquals('e', fiveChars.charAt(4),
		"Index 4 should be e"),
		() -> assertEquals('c', fiveChars.charAt(2),
		"Index 2 should be c")
	);
}

@test
public void emptyStringCharAtExceptionTest() {
	assertAll("Empty ioobe",
		() -> assertThrows(IndexOutOfBoundsException.class,
			() -> EMPTY_LITERAL.charAt(0),
			"Empty index 0"),
		() -> assertThrows(IndexOutOfBoundsException.class,
			() -> EMPTY_LITERAL.charAt(1),
			"Empty index 1"),
		() -> assertThrows(IndexOutOfBoundsException.class,
			() -> EMPTY_LITERAL.charAt(-1),
			"Empty index -1")
	)
}
```