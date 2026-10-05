# Successor Property
- if $n\in \mathbb{N}$ and $n\neq0$, then there is $m\in \mathbb{N}$ such that $n=m+1$. 
## New Definition of Natural Numbers
- We say that the natural numbers is the intersection of the subsets $S$ of $\mathbb{R}$ with the properties:
	- $1\in S$
	- if $x\in S$, then $x+1\in S$
- Slight rewrite of above principle,*Theorem 4.3.*: If,
	- $X\subseteq \mathbb{N}$
	- $0\in X$
	- $(\forall n\in \mathbb{N})n\in X\implies(n+1)\in X$
# Principle of Induction
- *Corollary 4.4*: For each $n\in \mathbb{N}$, let $P(n)$ be a mathematical statement. If properties (a) and (b) below hold, then $P(n)$ is true $\forall n\in \mathbb{N}$
	- $P(0)$ is true. *Base Case*
	- For every $k\in \mathbb{N}$, if $P(k)$ is true, then $P(k+1)$ is true. *Induction Step*
	- We call "$P(k)$ is true" the *induction hypothesis*
## A Classic Induction Proof
- Prove that for $n\in \mathbb{N}$,
$$
0+1+2+3+\dots+n=\frac{n(n+1)}{2}
$$
- Proof by mathematical induction. Base case: let $n=0$, we note that $\sum_{i=0}^ni=\frac{0(0+1)}{2}$. Induction Step: let $\sum_{i=0}^ki=\frac{k(k+1)}{2}$ (w.m.s.t $\sum_{i=0}^{k+1}i=\frac{k+1(k+2)}{2}$). Note that $\sum_{i=0}^{k+1}i=\sum_{i=0}^ki+(k+1)$. By the inductive hypothesis this implies $$\sum_{i=0}^{k+1}i=\frac{k(k+1)}{2}+(k+1)=\frac{k(k+1)}{2}+\frac{2(k+1)}{2}=\frac{k(k+1)+2(k+1)}{2}=\frac{(k+2)(k+1)}{2}$$
## Changing the Base Case
- *Corollary 4.9* Let $k\in \mathbb{Z}$, For each $x\in \mathbb{Z}$, Let $P(x)$ be a mathematical statement. If properties a and b below hold, then $P(n)$ is true $\forall n\in \mathbb{Z}$ such that $n\geq k$
	- $P(k)$ is true
	- $(\forall x\geq k)$ if $P(x)$ is true, then $P(x+1)$ is true.
# More Abstract Induction Proof
- *Lemma 4.11*: Let $N\in \mathbb{N}^+$ and, for $0\leq n\leq N$, $a_{n}\in \mathbb{R}$. if $c\in \mathbb{R}$, then
$$
\sum_{n=0}^Nca_{n}=c\left( \sum^N _{n=0}a_{n}\right)
$$
- distributive property on multiple terms.