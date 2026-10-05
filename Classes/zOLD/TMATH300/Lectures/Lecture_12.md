# Set of Functions
- Let $X$ and $Y$ be sets. The set of all function with domain $X$ and codomain $Y$ is written $Y^X$.
	- $|Y^X|=|Y|^{|X|}$
# An Uncountable Set
- *Proposition 6.8.* Let $X$ be a set and define $F:\lceil 2 \rceil^X\to P(X)$ such that for every $\chi \in \lceil 2 \rceil^X, F(\chi)=\chi^{-1}(1)$.  Then $F$ is a bijection
- *Theorem 6.9.* The set of infinite binary sequences is bijective with $P(\mathbb{N})$ and therefore uncountable
# Diagonalization Argument
- We can use the *Diagonalization Argument* to show that there cannot exist a surjection from the $\mathbb{N}$ to $\lceil 2 \rceil^\mathbb{N}$
Suppose $f:\mathbb{N}\to \lceil 2 \rceil^\mathbb{N}$ is a surjection. Define $\chi \in \lceil 2 \rceil^\mathbb{N}$ such that $\chi=a_{0},a_{1},a_{2},\dots$ where $a_{i}=\begin{Bmatrix}0\text{ if }f(i)=1 \\ 1\text{ if }f(i)=0\end{Bmatrix}$ . 
- *Theorem 6.11.* The set of infinite decimal expansions $\lceil 10 \rceil^\mathbb{N}$, is uncountable
- *Corollary 6.14.* $\mathbb{R}$ is uncountable
# Cantor's Theorem
- *Proposition 6.15.* Let $X$ and $Y$ be sets. Then there is a surjection $f:X\to Y$ if and only if $|X|\geq|Y|$
- *Theorem 6.16.* Let $\{ X_{n}|n\in \mathbb{N} \}$ be a family of sets such that $X_{n}$ is countable for all $n\in \mathbb{N}$, and let $X=\bigcup_{n\in \mathbb{N}}X_{n}$. Then $X$ is countable
	- Proven using the diagonal argument (not diagonalization argument)
- *Theorem 6.20.* Any cartesian product of countable sets is a countable set.
# Algebraic Real Numbers
- A real number $a$ is *algebraic* if there is a polynomial $p$ with integer coefficients such that $p(a)=0$. We shall denote the set of all algebraic numbers by $\mathbb{K}$.
- *Theorem 6.22.* $\mathbb{K}$ is countable.
# Transcendental Numbers
- *Corollary 6.23.* $\mathbb{K}\neq \mathbb{R}$
- A *transcendental number* is a real number that is not algebraic
- *Corollary 6.24.* There are uncountably many transcendental numbers.