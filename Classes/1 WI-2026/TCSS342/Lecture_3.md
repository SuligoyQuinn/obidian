# Trees
- Like linked lists trees consist of nodes that are connected to each other
	- Trees have any number of connections per node
	- In general graphs have any number of connections per node
- In a tree the connections have a direction
	- All edges point from a parent to a child
```java
public class Tree<Type> {
	private class Node {
		Type item;
		
		Node(Type item, Node next) {
			this.item = item;
			...
		}
		...
	}
	Node root;
	...
}
```
- Jargon
	- The root node of a tree is the node with no parent
	- A node with no children is called a leaf
	- All other nodes are internal/intermediate nodes
	- There is exactly one path of edges from the root node to any other node
	- The number of children a node has is called its out-degree
	- The number of parents a node has is always one
## Tree Terminology
- Node $A$ is an *ancestor* of a node $B$ if there exists a directed path from $A$ to $B$ in the tree
	- Then $B$ is the descendant of $A$
- The *depth* of a node is the length of the path from the root to the node
	- This is measured as number of edges (0 based) or number of nodes (1 based)
	- The depth of the tree is defined as the maximum depth of any node
- The *height* of a node is the length of the path from the node to the deepest leaf in its sub-tree
	- This is measured as number of edges (0 based) or number of nodes (1 based)
	- The height of the tree is defined as the height of the root
- The height of a tree is equal to the depth of a tree
## $m$-ary Trees
- an $m$-ary tree is a tree in which every parent is limited to at most $m$ children
- a *binary tree* is a tree in which every parent has at most $2$ children
	- left, right
- A *ternary tree* is a tree in which every parent has at most $3$ children
	- left, center, right
## Binary Trees
- two common types of binary trees
	- A *heap* maintains an ordering between parents and their children
	- A *binary search tree* maintains an ordering between all nodes for efficient search
## Complete Trees
- Def 1 A complete $m$-ary tree of depth $d$ is one in which every parent has exactly $m$ children except nodes at depth $d$
- Def 2 A complete $m$-ary tree of depth $d$ is one in which every parent has exactly $m$ children except nodes at depth $d$ and $d-1$.
### Complete Binary Tree
- How many nodes are there on depth $i$ of a complete binary tree
	- Assume root is depth $0$
	- $2^i$ nodes on level $i$
- How many nodes are there in a complete binary tree of depth $d$
	- $\sum^d_{i=0}2^i=2^{d+1}-1$
- What is the depth of a complete binary tree with $n$ nodes
	- $\lfloor \log_{2}n \rfloor$
## Tree Traversal
- Unlike list there is not single canonical ordering of the nodes in the tree
- pre-order
	- Operate, traverse left, traverse right
- in-order
	- Traverse left, operate, traverse right
- post-order
	- Traverse left, traverse right, operate
[1,2,3]
[3,1,2]