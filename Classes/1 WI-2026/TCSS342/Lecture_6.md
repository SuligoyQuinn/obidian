# Binary Search Trees
- binary tree with the following invariant
	- Elements in the left sub-tree of a node have values smaller than the values of the node
	- Elements in the right sub-tree of a node have values larger than the value of the node
## Benefits of BST structure
- An in-order traversal of a BST will display the contents of the BST in order
- Searching for an element in a BST will mimic a binary search
	- cost of each individual search is equal to depth of element
## Adding to a BST
- When we add a new node to a BST we must ensure that we don't violate the invariant
- In BST we do this by searching for the element and placing it in the (presumably) empty position we find
## Removing from a BST
- Removing an item begins with a search for the item
- Once found we can remove it easily in two cases
	- If it is a leaf we can remove it freely without disturbing the tree
	- If it only has one child we can remove it and promote its only child to its position
- To remove a node with two children, replace it with either the smallest element in the right sub-tree, or the largest element in the left sub-tree
## Depth of a BST
- a BST depth depends on the order in which we add elements
- All BST operations take time $O(d)$
	- in the worst case this is $O(n)$
	- In the best case this is $O(\log n)$