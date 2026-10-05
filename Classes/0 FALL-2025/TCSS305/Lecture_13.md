# Creating Menu Bars
```java
final Jframe frame = new Jframe("TestBar");


// Helper Method that adds our test buttons to the JMenuBar
private JmenuBar createMenu(final Jframe theFrame) {
	final JMenuBar menuBar = new JMenuBar();
	
	menuBar.add(buildFileMenu(theFrame));
	menuBar.add(buildColorButtonMenu());
	menuBar.add(buildLogginMenu());
	
	return menuBar;
}

private JMenu buildFileMenu(final JFrame theFrame) {
	final JMenu menu = new Jmenu = new JMenu("File");
	// Mnemonic for fast access
	menu.setMnemonic(KeyEvent.VK_F);
	final JMenuItem exitItem = new JMenuItem("Exit");
	
	// Exit functionality
	exitItem.addActionListener(theEvent ->
		System.exit(99)); // Bad Exit
		theFrame.dispatchEvent(new WindowEvent(theFrame, 
				WindowEvent.WINDOW_CLOSING)) // Good Exit
	menu.add(exitItem);
	return menu;
}
```

# Painting Components
```java
@Override
public void paintComponent(final Graphics theGraphics) {
	super.paintComponent(theGraphics);
	// Cast to better graphics library
	final Graphics2D g2d = (Graphics2D) theGraphics;
	
	// Antialiasing on for better circles
	g2d.setRenderingHint(RenderingHints.KEY_ANTIALIASING,
						RenderingHints.VALUE_ANTIALIAS_ON);
	
	final Shape rectangle = 
				new Rectangle2D.Double(getWidth() - RECTANGLE_WIDTH /2.0,
							getHeight() - RECTANGLE_HEIGHT / 2.0,
							RECTANGLE_WIDTH * 2, RECTANGLE_HEIGHT * 2);
	g2d.setPaint(Color.RED);
	g2d.setStroke(new BasicStroke(10));
	
	g2d.draw(rectangle);
	g2d.setPaint(Color.BLUE);
	g2d.fill(rectangle);
}
```
