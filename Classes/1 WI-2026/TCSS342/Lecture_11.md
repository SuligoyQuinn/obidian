# B-Trees
## Invariant
- A B-Tree is a generalization of a binary search tree
	- Defined to have an order $d\geq 0$
- Each node has at most $d$ keys and at most $d+1$ children
- Every node except the root has a minimum of $\left\lceil  \frac{d}{2}  \right\rceil$ keys
- The number of children is always the number of keys plus one, or none in the case of leaves
## Variant B+-Trees
- Only leaf nodes contain values
- When $B^+$-Tree is used as a Map, the keys are used for navigation only
## Insert
- Splitting a full node
	- First add the entry to the full node
	- Split overflow node into two nodes along the middle entry and promote the middle entry to the parent node
	- When splitting root, create a new parent node
- $B^+$-Tree note
	- If node we are splitting is leaf then middle node must also appear in one of the two new leaf nodes and so is copied up
## Redistribution
- Variant of the insertion algorithm will attempt redistribution before splitting node
	- helps keep height small by increasing occupancy
- If node has too many entries after insert we check its siblings for room
	- check immediate siblings (left and right)
	- if either sibling can accommodate an extra entry we shuffle entries over to make room for new entry
	- requires editing the node, its chosen sibling and their parent node, but no splitting
## Deletion
- To delete an entry we must first find the leaf that contains it
- In common case we remove entry from page
- If entry is on page with minimum occupancy
	- first option is to redistribute
	- if both adjacent siblings are also at minimum occupancy then we can do a merge
		- both siblings will have $d$ entries before the merge, we can borrow one entry from parents to make fully occupied node with $d + (d-1) + 1=2d$ entries
	- if last entry of root is deleted an entry from its children can be promoted to root, if those children already at minimum occupancy, can be merged and the root removed altogether causing height of tree to be reduced by one