# Comparing the Size of Sets
- Let $X$ and $Y$ be sets. We say that $X$ and $Y$ have the same cardinality if a bijection $f:X\to Y$ exists.
- We can express that two sets have the same cardinality by $|X|=|Y|$
	- We say that the sets are *equinumerous*
## Finite and Infinite
- We say that a set $X$ is *finite* if there is a bijection from $f:\lceil n \rceil\to X$ for some $n\in \mathbb{N}$. A set is *infinite* if no such bijection exists.
- *Proposition 6.1.* There is a bijection $f:\lceil m \rceil\to \lceil n \rceil$ if and only if $m=n$
- *Corollary 6.3* if $X$ is finite, then for exactly one $n$ there is a bijection from $X$ to $\lceil n \rceil$.
# Natural Numbers
- *Theorem 6.5.* $\mathbb{N}$ is an infinite set.
- *Theorem 6.6.* if $X$ is infinite, then there exists an injective function $f:\mathbb{N}\to X$
	- We know $X$ is non-empty and so let $x_{0}\in X$. And define $f:\mathbb{N}\to X$, so then $f(0)=x_{0}$ then choose $x_{1}\in X/x_{0}$ and let $f(1)=x_{1}$. Suppose for $k\in \mathbb{N}$, $f(k)=x_{k}$ for some $x_{k}\in X$.
	- Natural numbers are the smallest infinite set
- If there exists a bijection between any set $X$ and $\mathbb{N}$, then we say that the cardinality of $X$ is $\aleph_{0}$
# Countable Sets
- If a set is finite or has cardinality $\aleph_{0}$ it is called a *countable set*
# Uncountable Sets
- If a set is not countable then it is *uncountable*
- *Corollary 6.14.* The $\mathbb{R}$ is uncountable
# Some Notation
- Let $X$ and $Y$ be sets.
- We write $X\preccurlyeq Y$ if there is an injection $f:X\to Y$.
- We write $X\prec Y$ if $X\preccurlyeq Y$ and $|X|\neq|Y|$
# Power Sets
- Let $X$ be a set. Then $P(X)=\{ Y|Y\subseteq X \}$ is called the *power set* of $X$. It is the set of all subsets of $X$.
- Example: power set of $X=\{ a,b,c \}$ is $\{ \{ a,b,c \},\{\emptyset  \},\{ a \},\{ b \},\{ c \},\{ a,b \},\{ a,c \},\{ b,c \} \}$
- *Theorem 6.7.* Let $X$ be a set. Then $|X|<|P(X)|$
	- Means $|\mathbb{N}|<|P(\mathbb{N})|$
		- Powerset of natural numbers is uncountable
