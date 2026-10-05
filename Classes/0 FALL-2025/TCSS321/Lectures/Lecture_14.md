# More Pseudo Code
- Selection Sort
```java
Input: An array A[1...n] of real numbers, n>=2
Output: A[1...n] with the orinal elements of A in sorted (non decreasing) order

selectionSort(A[1...n])
	for i <- 1 to n-1 do
		// find min of A[i...n]
		minIndex <- i
		for j <- i+1 to n do
			if A[j] < A[minIndex] then
				minIndex <- j
		temp <- A[minIndex]
		A[minIndex] <- A[i]
		A[i] <- temp
```
# Big-Oh notation
- Let $f$ and $g$ be functions from the set of real numbers to the set of real numbers
	- $f(n)$ is $O(g(n))$ if there are constants $c$ and $k$ such that $f(n)\leq c\cdot g(n)$ for all $n>k$
- 
