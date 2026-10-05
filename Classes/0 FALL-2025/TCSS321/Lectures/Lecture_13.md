# Pseudo Code
- Simple algorithm using pseudo code
```python
Input: An array A[1...n] of integers
Output: The maximum element in A
maximum(A[1...n])
	max <- A[1]
	for i <- 2 to n do
		if max < A[i] then
			max <- A[i]
	return max
```

```python
Input: An array A[1...n] of integers
Output: The sum of all integers in A
sum(A[1..n])
	sum <- A[1]
	for i <- 2 to n do
		sum = sum + A[i]
	return sum
```

```python
Input: An array A[1...n] of integers, and an integer key
Output: Smallest index i such that A[i] = key, or -1
find(A[1...n], key)
	i <- 1
	while (i <= n and A[i] != key)
		i <- i + 1
	if i > n then
		return -1
	else
		return i
```
hi
