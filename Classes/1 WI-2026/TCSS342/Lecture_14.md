# Text Search
- Given two character strings $T[0\dots n-1]$ and $S[0\dots m-1]$ with $n \gg m>0$, the text search problem consists of finding all positions $i_{1},\dots,i_{p}$ such that string $S$ occurs at all of those positions on $T$
	- $\forall 0\leq k\leq p | T[i_{k},\dots,i_{k}+m-1]=S$
## Rabin-Karp text search
- Idea: pre-process $T$ instead
- For simplicity assume initially that all searched patterns are of length $m$
- Then hash all sub-strings of length $m$ that occur on $T$ at all viable indices
- Add positions where those sub-strings occur to a chaining collision list
	- initialize all buckets of a hash table $rk$ to empty lists
- For all indices $0\leq i\leq n-m$
	- Denoting the sub-strings of length $m$ located at index $i$ on $T$ by $T[i:m]$, compute the bucked ID $k=hash(T[i:m])$
	- The list at that bucket ID is thus `rk.get(k)`
	- Now append the index value $i$ to that chaining list
- Unrealistic to assume all strings have same length