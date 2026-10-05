# Linked Lists
- A linked list is structure of nodes where each node is linked to others by storing the addresses of other nodes
	- Allows for dynamic growth because every time element is added, new node is allocated somewhere in memory and is linked
	- Worst case cost of adding to end of linked list is $O(1)$
	- Drawbacks
		- Given up random access
		- If we want item $i$ we must traverse the links to get there in $O(i)$ time.
# Searching a List
- Finding an element in a list is a standard problem
	- If list is unsorted we must check every location $(O(n))$
- If list is sorted we can binary search $(O(lg n))$
