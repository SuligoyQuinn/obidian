# Tree Maps
- Efficient way to implement map is with BST
- Would yield $O(\log n)$ operations
- Hash tables yield $O(1)$ operations
	- Cannot traverse table in order
# Hash Functions
- Hash table has $n$ buckets where each bucket could potentially hold a value
- Hash function must produce a bucket ID
- Hash functions must obey following assumptions
	- Equal object must always return the same integer
	- Every integer should be mapped as evenly as possible
- When two keys are mapped to the same index, they cause a collision
