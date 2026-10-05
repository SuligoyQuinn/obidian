# AVL Trees
## Defining Balance
- Each node is assigned a balance factor equal to the difference in height between its left and right sub-trees
## Maintaining Balance
- The invariant of AVL trees is that the balance factor of every node must be $-1,0,1$
- Imbalance can only be introduced when we add or remove nodes
	- thus must modify methods to check for and correct imbalance
- When we remove a node, imbalance can only be created in nodes along the path from that node to the root
## Rotating a Node
- A rotation redirects a few edges, keeping relative order of the nodes unchanged
- The parent of a node is demoted to one of its two sub-trees, and the child from the opposite side is promoted to parent position
```java
rotateL() {
	Node A = this;
	Node B = A.rchild;
	A.rchild = B.lchild;
	B.lchild = A;
	return B;
}

rotateR() {
	Node A = this;
	Node B = A.lchild;
	A.lchild = B.rchild;
	B.rchild = A;
	return B;
}
```

