# The Union-Find Problem
- Consider the problem of maintaining a dynamical collection of disjoint sets of integers from range $0\dots N-1$
- Following Operations must be supported
	- Initializing the collection with individual sets covering the whole range
	- Finding which set contains an element
	- Replacing two sets by their union
# Upward-pointing trees
- All nodes but the root have one and only one parent, so a single pointer is needed per node
# Implementing Union-Find
- Initialization
	- Each integer in range $0\dots N-1$ starts in its own set
	- Name each set after the smallest contained value
- Finding
	- Keep a map from integer values to tree nodes
	- The set containing a key $k$ is the root of the tree containing the leaf `map.get(k)`
- Union
	- "Union $k$ and $l$" invokes Find twice and makes the larger node descend from the smaller
- Drawback: path from leaf to root may be long
## Path Compression
- Solution
	- In every find operation, when visiting any node $p$ make it point directly to its grandparent instead of its current parent