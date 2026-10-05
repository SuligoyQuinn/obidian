# Red-Black Trees
- Another kind of self balancing BST
- Following additional invariants
	- A node is either red or black
	- The root is black
	- All leaves are black and contain no data
	- Every red node has black children
	- The number of black nodes is the same along any path from the root to a leaf. This is called the black depth of the tree
## Adding to Red-Black Trees
- Search from root
	- Search ends at a black leaf
	- Replace it with a red node with two black children
	- Then restore the invariant
- Case 1: parent is black
	- Invariant holds
- Case 2: parent and its sibling are red
	- Repaint the parent and its sibling black and the grandparent red
	- This might make a red node have a red child if great-grandparent is red
	- Must recursively fix this on grandparent node if this is the case
- Case 3: The root becomes red
	- Repaint it to black
- Case 4: Parent is red but its sibling is black
	- Sub-case 1: New node and parent are right children (or left children)
	- Sub-case 2: New node is left child and its parent is right child (or vice versa)
### LL Balancing
- Color g left black and redirect to s
- Color p right red and redirect to g
- Redirect root to p
### RR Balancing
- Color g right black and redirect to s
- Color p left right and redirect to g
- Redirect root to p