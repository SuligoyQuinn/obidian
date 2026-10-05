# Balanced Binary Tree
## The Balance Problem
- In simple BST there is no control over the tree structure during insertions or deletions
- A self-balancing binary tree is a binary search tree with the following additional invariant
	- The binary search tree must be balanced
		- A tree is perfectly balanced if
		- Its left and right sub-trees are themselves perfectly balanced
		- The numbers of nodes of its sub-trees differ by at most 1 
- Adding new elements
	- Transfer root to largest element on the left
	- Transfer smallest element from the right sub-tree to the root.
	- Recursively use same algorithm on left and right sub-trees