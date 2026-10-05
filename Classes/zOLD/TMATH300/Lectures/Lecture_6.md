# Proving Universal Statements
## Classic Proof by Contradiction
- Proof that $\sqrt{ 2 }$ is irrational
	- Using a proof by contradiction, assume that $x$ is a rational number, and also assume that $x^2=2$; we wish to derive a logical contradiction. Write $x=\frac{m}{n}$, where $m$ and $n$ are non-zero integers that have no common factors. Then $x^2=\frac{m^2}{n^2}=2$. So $m^2=2n^2$. Therefor $m^2$ is even, then by Example 3.21, $m$ is even. Therefore $m=2k$ for some integer $k$, and so $m^2=4k^2=2n^2$. Therefore $n^2=2k^2$ is even, so $n$ is even. But then both $m$ and $n$ are even, and so have $2$ as a common factor, which contradicts the assumption that $\frac{m}{n}$ was the reduced form of the rational number $x$. q.e.d
# Negations
- Negations follow DeMorgan's Law
	- $\sim(PandQ)=\sim Por \sim Q$
	- $\sim(PorQ)=\sim Pand\sim Q$
## Negations of Quantifiers
- $\sim(\forall x)P(x)=[(\exists x)\sim P(x)]$
- $\sim(\exists x)P(x)=[(\forall x)\sim P(x)]$
- Ex) $\sim((\forall \in \mathbb{Z})x^2>x)=(\exists \in \mathbb{Z})x^2\leq x$
# Proving Existential Statements
- Construction Proof
	- Proof that there exists a function $f:\mathbb{R}\to \mathbb{R}$ whose first derivative is everywhere positive and whose second derivative is everywhere negative
	- $1-e^-x$
- Counting Proof
	- Suppose that there are at least 30 students in a class, show that at least two students share the same last initial
	- Only 26 possible initial, 4 students have shared initials
	- Pigeon-hole Principle: If there are more letters than pigeon-holes then at least one pigeon-hole must have more than one letter
- Contradiction
	- Suppose all the points in the plane are colored either red or blue. Prove that there must be two points of the same color exactly one unit apart
	- Assume there are no two points of the same color exactly one unit apart. Imagine an equilateral triangle with side length 1. There are three points all 1 unit apart, at least two must share a color.