# More pseudo code induction
```java
Input: positive integer n
Output: n!
factorial(n)
	result <- 1
	for i <- 1 to n do
		result <- i * result
	return result
```
- Claim: After the $i^{th}$ iteration of the for loop $(1\leq i\leq n)$, the variable result contains the value $i!$.
- Proof: Proof is by induction on $i$. Let $P(i)$ be the statement "After the $i^{th}$ iteration of the for loop, result contains $i!$". Basis step: $i=1$. Before the for loop, result contains $1$, and after the first iteration result contains $1\cdot1=1!$. Induction hypothesis: Suppose that for some fixed $i\geq1$, $P(i)$ is true. That is, for some fixed $i\geq 1$, after the $i^{th}$ iteration, result contains $i!$. Induction Step: We need to show that after the $(i+1)^{th}$ iteration, result contains $(i+1)!$. In the $(i+1)^{th}$ iteration, result is assigned to $(i+1)\cdot result$. After the $i^{th}$ iteration, result contains $i!$ (by the I.H). So, at the end of the $(i+1)^{th}$ iteration, result contains $(i+1)\cdot i! =(i+1)!$. Q.E.D
# Matrices and Relations
- Let $A$ and $B$ be sets. A binary relation from $A$ to $B$ is a subset of $A\times B$.
- Relations
	- Reflexive
		- if for all $a\in A$, $(a,a)\in R$
	- Symmetric
		- if for all $a,b\in A$, $(b,a)\in R$ if $(a,b)\in \mathbb{R}$
	- 