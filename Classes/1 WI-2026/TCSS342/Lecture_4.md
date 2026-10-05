# Priority Queue
- Two relevant operations
	- offer/add/enqueue
		- Adds new element to the queue
	- poll/remove/dequeue
		- Removes and returns element with the highest priority
- Want to implement so these are as efficient as possible
	- Use unordered list
		- Adding new elements: $O(1)$
		- Finding maximum to remove: $O(n)$
	- Use ordered list
		- Adding new elements to correct place: $O(n)$
		- Removing last element of the list: $O(1)$
		- 
# Heap
- A (binary) *heap* is a (binary) tree satisfying this invariant
	- Heap property
		- The priority of the item stored at a parent node is higher than the values of the items stored at its child nodes
	- Complete Left-Loaded Binary Tree
		- Every level of the heap is full except possibly the last level which is left-loaded
## Adding to Heap
- In a complete binary tree there is exactly one place we can add a new item without violating invariant
	- First non-empty level on the left
- If new element lower priority then parent then do nothing
	- Otherwise sift up by swapping with parent until invariant holds
## Remove From Heap
- Always remove root node then promote another node to be the new root
	- Swap root with right most element on deepest level, then remove, then bubble up
## Array Implementation
- Children of a node at position $i$ are at positions $2i+1$ and $2i+2$
- Parent of a node at position $i$ is at position $\left\lfloor  \frac{i-1}{2}  \right\rfloor$
## Creating a Heap
- If a complete left-loaded binary tree is not a heap, we can make it a heap by testing and enforcing the heap condition for every node in sequence
	- In worst case each new node has to be sifted up to the root
		- $O(n\log n)$
- *Floyd's Algorithm*
	- Create a complete left-loaded binary tree containing all desired elements
		- Just create an array of all elements
	- The second half of the array (deepest level) is already a collection of heaps
		- If node has no children, by vacuity, it is a heap
	- Move from right to left and up the heap, combining the left and right sub-heaps of each node met along the way
	- After a swap, check the swapped child's sub-tree
	- $O(n)$
