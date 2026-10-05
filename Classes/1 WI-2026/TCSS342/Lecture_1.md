# Abstraction
- What is abstraction
	- refers to the world of ideas
	- in contrast to physical world which is called the concrete
- Ex
	- A blueprint is an abstraction and the building is the concrete
	- An algorithm is an abstraction and the program is a concrete
- *Abstraction* is the process of eliminating details to obtain a concise conception or model of some entity, or process.
- *Concretization* is the process of filling in details of a model or concept so as to arrive at a real world product of the abstraction
## Abstract Data Types
- List
	- Array, Array List, Linked List, Stack, Queue
- Tree
	- Binary Search Tree, AVL Tree, B-Tree, Binary Heap, Huffman Tree
- Map/Dictionary
	- Hash Tables, Chaining, Probing, Cuckoo Hashing, Extendible Hashing
- Graphs
	- Undirected, Directed, Weighted, Connected, Bipartite and Complete Graphs
# List
- List Invariant: A list is a collection of objects in some one-dimensional order
- If we have a collection of objects with no particular order we have a set
- List can be further defined by its access criteria through additional invariants
	- Stack Invariant: LIFO
	- Queue Invariant: FIFO
	- Array(Vector) Invariant: Index Access
	- Linked List Invariant: Iterator Access
## Array
```java
int[] ints = new int[n]
```
- Allocates enough memory in sequence to store $n$ integers.
	- Each integer in java takes 32 bits, or 4 bytes
	- In total we have $4\cdot n$ bytes
- Segment of memory then used to store the entire array of integers
	- Address of the array is address of the first element
	- Can calculate address of any element in the array with some math
		- Address of array $\text{ints}+4\cdot \text{index of element}$
	- Called random access
## Dynamic Arrays
- Dynamic arrays will begin with initial capacity
	- Capacity can initially be set to just 1
		- Typically small power of $2$
- Elements can be added in a simple fashion when the size is less than the capacity which takes $O(1)$ time
- If addition exceeds capacity then create distinct array with double size which takes $O(n)$ time
### Amortized Constant Time
Adding $N$ elements to a new array list, where $N$ is large
- Say $N=100$ and we start with an array of capacity one.
	- Cost of $100$ additions is $100$.
	- Cost of doubling will first be $1$ then $2$ and so on until $N$ fits the capacity
	- $1+2+4+8+16+32+64=127$
	- Total cost is $227$
		- Amortized time is $2.27$
- Say $N=1024$
	- Cost of $1024$ adds is $1024$
	- Cost of doubling is $\sum^9_{i=0}2^i=1023$
	- Total cost is $2047$
		- Amortized time is $1.999$
- General Proof
$$
N+\sum^{\lceil \lg N \rceil -1}_{i=0}2^i=N+2^{\lceil lgN \rceil}-1<N+2^{lgN+1}=3N
$$