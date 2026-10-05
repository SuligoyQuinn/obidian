# Quotient Space
- Refer to the set of equivalence classes $\{ [x]_{R}|x \in X \}$ as the *quotient space*, *X/R*, of $X$ by $R$
- for any equivalence relation $R$ on a set $X$, when $x\sim y$ we can also say $x\equiv y$
# Properties of Equivalence Classes
- if $\sim$ is an equivalence relation on $X$ and $x,y\in X$,
	- if $x\equiv y$ then $[x]=[y]$
	- if $x\not\equiv y$ then $[x]\cap[y]=\varnothing$
# Partitions
- Let $\{ X_{a}|a\in A \}$ be a family of sets. The family is *pairwise disjoint* if for any $a,\beta \in A,a\neq \beta$, then $X_{a}\cap X_{\beta}=\varnothing$
- If the union of a family of pairwise disjoint non-empty subsets $F$ of the set $Y$ equals all of $Y$ then we call $F$ a *partition* of $Y$
- Every equivalence relation $\sim$ on a set $X$ forms a partition of $X$ and every partition of $X$ can be turned into an equivalence relation
# S0me Number Theory
- Let $a,b\in \mathbb{Z}$. We say that *a divides b*, $a|b$, if there is $c\in \mathbb{Z}$ such that $a\cdot c=b$
- An integer $a$ is *prime* if and only if there are exactly two positive integers that divide $a$
- We say that $a$ and $b$ are *coprime/relatively prime* if and only if $gcd(a,b)=1$
# Congruence
- Let $x,y,n\in \mathbb{Z}$ and $n>1$. Then $x\equiv y$ mod $n$ if $n|(x-y)$
- This relation on $\mathbb{Z}$ is called *congruence mod n*
- The equivalence classes of $\equiv_{n}$ are called *congruence classes*, *residue classes*, or *remainder classes mod n*
- This set of congruence classes  mod $n$ is written as $\mathbb{Z}_{n}$ or $\frac{\mathbb{Z}}{n\mathbb{Z}}$
# Modular Arithmetic
- If $a\equiv_{n}r$ and $b\equiv_{n}s$, then $a+b\equiv_{n}r+s$ and $ab\equiv_{n}rs$
# Big Hint for 2.19
- 8 equivalence classes for $\mathbb{Z}_{8}$, for each of these equivalence classes, $[n]_{8}$, find the equivalence class of $n^2$ 
$$\mathbb{Z}_{8}=\{ [0]_{8},[1]_{8},[2]_{8},[3]_{8},[4]_{8},[5]_{8},[6]_{8},[7]_{8}\}$$
$$
\mathbb{Z}^2_{8}=\{ [0]_{8},[1]_{8},[4]_{8},[1]_{8},[0]_{8},[1]_{8},[4]_{8},[1]_{8}\}
$$
- all numbers fall into first congruence classes, all numbers squared fall into second congruence classes
# Restricted Domains
- Let $f:X\to Y$ and $W \subseteq X$. The *restriction of  f to W*, written $f|_{W}$, is the function $f|_{w}:W\to Y$
# Getting Started on 2.22
- Let $X$ be the set of functions from finite subsets of $\mathbb{N}$ to $\lceil 2 \rceil$.
- 3 elements of X
	- $W=\{ 0,1,2 \}, f:W\to \lceil 2 \rceil =\{ (0,0),(1,1),(2,0) \}$
	- $W=\{ 3,1,2 \}, f:W\to \lceil 2 \rceil =\{ (3,0),(1,1),(2,0) \}$
	- $W=\{ 0,100,2, 5 \}, f:W\to \lceil 2 \rceil =\{ (0,0),(100,1),(2,0),(5,1) \}$
	- W is just some defined set of natural numbers, doesn't really matter what as long as it ends
	- f just has to map to $\lceil 2 \rceil$ aka $\{ 0,1 \}$
- Define a relation $R$ on $X$ as follows: if $f,g\in X$, then $fRg$ if and only if $Dom(g)\subseteq Dom(f)$ and $g=f|_{Dom(g)}$.
	- Where g is defined, f and g have the same output
	- f has potentially bigger output
- Identify an $f,g\in X$ such that $fRg$
	- $W=\{ 0,1,2 \}, Z=\{ 0,1 \}, f:W\to \lceil 2 \rceil=\{ (0,1),(1,0),(2,1) \},g:Z\to \lceil 2 \rceil=\{ (0,1),(1,0)\}$
# Getting Started on 2.23
- Give an example of an infinite binary sequence
	- can't do that unless described by pattern
		- most aren't
	- All zeroes/ All ones
- Let $X$ be the set of all infinite binary sequences. Define a relation $R$ on $X$ as follows: if $f,g\in X$, then $fRg$ if and only if $f^{-1}(1)\subseteq g^{-1}(1)$