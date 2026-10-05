# Set Operations
- Given sets $A$ and $B$, their *intersection* $A\cap B$ is the set containing every element that appears both in $A$ *and* $B$
	- If $A\cap B = \varnothing$ they are disjoint
- Their *union* $A \cup B$ is the set containing every element in $A$ *or* $B$.
- If a set contained within a well-defined maximum set or *universe U* then we say that the *complement* of $A$, or $A^c$, is all elements of $U$ not in $A$
## Example
### Let $X$ and $Y$ be subsets of some set $U$. Prove that $(X\cup Y)^c=X^c\cap Y^c$
---
$$
\text{Let } a \in(X\cup Y)^c. \text{[w.m.s.t. }a\in X^c\cap Y^c]
$$
$$
\text{Since }a\in(X\cup Y)^c\text{ then }a\not\in X \text{ and }a\not\in Y

$$
$$
\text{so }a\in X^c\cap Y^c
$$
$$
\text{Let }a\in X^c\cap Y^c.\text{ [w.m.s.t } a\in(X\cup Y)^c]
$$
$$
\text{Since }a\in X^\cap Y^c\text{ then }a\not\in X\text{ and }a\not\in Y
$$
$$
\text{so }a\in(X\cup Y)^c
$$
$$
\text{q.e.d}
$$
# New Sets from Old Sets
- The *Cartesian product* of sets $S$ and $T$ is the set of all ordered pairs (2-tuples) with the first element in $S$ and the second element in $T$
	- In this case order matters.  $(1,2)\neq(2,1)$
	- $S=\{a,b\}\text{ and }T=\{c,d,e\}$
		- $S\times T=\{(a,c),(a,d),(a,e),(b,c),(b,d),(b,e)\}$
	- $|A\times B|=|A|\times|B|$
		- Size of product is product of sizes
	- Let $n\in \mathbb{N}^{+}, \text{ and }X_{1},X_{2},\dots,X_{n}$ be sets. The cartesian product of $X_{1},\dots,X_{n}$ is the set $X_{1}\times X_{2}\times\dots \times Xn=\{ (x_{1},x_{2},\dots,x_{n}) \}$
# Functions
- A function $f$ from a set $A$ to a set $B$ assigns a unique element $f(a)\in B$ to each element $a\in A$. We say that $f(a)$ is the *image of a under f*
- For $f:A\to B,A$ is the *domain* and $B$ is the *codomain*.
- The *range* of $f$, or $Ran(f)$, is $\{ f(x) | x \in A \}$
## Three Properties of Functions
- A function $f:A\to B$ is *injective* if for each $b\in B$ there is at most one $x \in A$ such that $f(x)=b$.
	- same as *one-to-one*.
	- if $x_{1}\neq y_{1}$, then $f(x_{1})\neq f(y_{1})$.
	- if $f(x_{1})=f(x_{2})$, then $x_{1}=x_{2}$
- A function is *surjective* if for each $b\in B$ there is at least one $x \in A$ such that $f(x)=b$.
	- codomain = range
- A function is *bijective* if for each $b\in B$ there is exactly one $x \in A$ such that $f(x)=b$.
	- Both injective and surjective
	- Function has an inverse
## Inverses
- a *bijection* $f$ always has an *inverse* $f^-1$
	- defined as $f^-1:B\to A$ such that for each $b\in B,f^-1(b)$ is the unique element $A$ such that $f(x)=b$.
- Function has an inverse if and only if it is a bijection