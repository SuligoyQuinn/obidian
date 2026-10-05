# Ideals in $\mathbb{Z}$
- If $I\subseteq \mathbb{Z}$ and $I\neq \emptyset$, then we call $I$ an *ideal of the integers* if it meets conditions
	- If $n,m\in I$ then $n+m\in I$
	- If $n\in I$ and $v\in \mathbb{Z}$ then $v \cdot n\in I$
# Ideals in $\mathbb{R}[x]$
- Same conditions but $\mathbb{R}[x]$ instead of $\mathbb{Z}$
# Principle Ideals in $\mathbb{Z}$
- An ideal $I$ in $\mathbb{Z}$ is *principle* if $\exists n\in \mathbb{Z}$ such that $I=\{ m\cdot n|m\in \mathbb{Z} \}$
- we call $n$ a generator of $I$ 
- *Theorem 7.23.* Every ideal of $\mathbb{R}[x]$ is principle
	- can use division algorithm to prove
# Why Real Numbers
- rational numbers form holes in number line
# Natural Numbers Revisited
- Let $Y$ be a set. The *successor function*, $S$, is defined by $S(Y)=Y\cup \{ Y \}$.
- Let $S$ be the successor function and $X$ be any collection of sets satisfying the following conditions
	- $\emptyset \in X$
	- $[Y\in X]\implies[S(Y)\in X]$
	- Then $X$ is called an *inductive set*
- Let $X$ be any inductive set. The set of *natural numbers* is the intersection of all subsets of $X$ that are inductive set
## Link traditional natural number definition
- $f(0)=\emptyset$
- For any $n\in \mathbb{N}$, $f(n+1)=S(f(n))$
## Operation of Natural Numbers
- If $m,n\in \mathbb{N}$, then we define addition by
	- $m+n=|(\lceil m \rceil \times \{ \lceil 0 \rceil \})\cup(\lceil n \rceil\times \{ \lceil 1 \rceil \})|$
- If $m,n\in \mathbb{N}$, then we define multiplication by
	- $m\cdot n=|\lceil m \rceil\times \lceil n \rceil|$
- If $m,n\in \mathbb{N}$, then we say
	- $[m\leq n]\iff[\lceil m \rceil\subseteq \lceil n \rceil]$
- Under new definitions, addition and multiplication still have commutative, associative, and distributive properties
# Integers and Rational Numbers
- Need for additive inverses leads to construction of integers. We use equivalence relation to define integers as equivalence classes of $\mathbb{N}\times \mathbb{N}$
	- Define an equivalence relation, $\sim$ on $\mathbb{N}\times \mathbb{N}$ such that $(m_{1},n_{1})\sim(m_{2},n_{2})\iff m_{1}+n_{2}=m_{2}+n_{1}$
	- We define $\mathbb{Z}$ to be $\mathbb{N}\times \mathbb{N}/\sim$
- Need for multiplicative inverse leads to construction of rational numbers. We use an equivalence relation to define integers as equivalence classes of $\mathbb{Z}\times \mathbb{Z}$
	- Define an equivalence relation, $\sim$ on $\mathbb{Z}\times \mathbb{Z}$ such that
		- $(a,b)\sim(c,d)\iff ad=bc$
		- We define $\mathbb{Q}$ to be $\mathbb{Z}\times \mathbb{Z}/\sim$