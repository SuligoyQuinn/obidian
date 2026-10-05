# Splay Trees
- Binary Search tree with the following invariant
	- The most recently searched element is at the root
- Maintenance idea
	- Perform a normal search for the given element
	- then rotate the tree so as to promote the root of the sub-tree where the search was made
## Splaying
- Try and keep recently searched elements close to the root
- Not balanced
## Bottom-up vs Top-down splaying
- Instead of rotating the found element up from the bottom
- A top down approach is possible
	- Since we know the root of the sub-tree will eventually get promoted, promote it right away
	- restart search from promoted root