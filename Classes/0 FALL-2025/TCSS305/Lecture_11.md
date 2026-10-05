# GUI
# Event Handler 
- user interactions registered as event
- EDT (Event Dispatch Thread)
	- loop running waiting to capture events from the operating systems
	- Listens for user and system events
```java
private void addListeners() {
	// Inner Class defined within another class
	myHelloButton.addActionListener(new HelloButtonActionListener());
	// Anonymous Class passed in as argument
	myGoodbyeButton.addActionListener(new ActionListener() {
		@Override
		public void actionPerformed(ActionEvent e) {
			myMessageLabel.setText("Goodbye");
		}
	});
	// Lambda expression passed in as argument
	myLambdaButton.addActionListener((theEvent) -> 
	myMessageLabel.setText("Kewl"));
}
class HelloButtonActionListener implements ActionListener {
	@Override
	public void actionPerformed(ActionEvent e) {
		myMessageLabel.setText("Hello World!");
	}
}
```
# Lambda Expressions
- Requirements for replacing
	- Expecting an object that implements an interface
	- Interface needs to have exactly one implementable method
- Parameter list
	- No Types
	- No parameters
		- `() ->`
	- 1 parameter
		- `(theParam) ->`
		- `theParam ->`
	- 2 or more parameter
		- `(theP1, theP2, theP3) ->`
- Arrow function
- Statement list
	- Try to be one statement
	- One statement
		- `() -> statement`
	- 2 or more statements
		- `() -> {statement; statement2;}`
- Returning values
	- One statement
		- `() -> 2+3`
	- 2 or more statements
		- `() -> {statement; statement2; return 2+3;}`
- 