# Sequences
- *finite sequence*, $\langle a_{n}|n<N \rangle$, is a function with domain $\lceil N \rceil$, where $N\in \mathbb{N}$
- *infinite sequence*,$\langle a_{n}|n\in \mathbb{N}\rangle$, is a function with domain $\mathbb{N}$.
# Infinite Union of Sets
- *infinite union*, $\bigcup^{\infty}_{n=1}X_{n}$, where for $n\in \mathbb{N}^+,X_{n}$ is a set
# Relation
- Given sets $A$ and $B$, a *relation R* is a subset of $A\times B$.
	- if $(a,b)\in R$, then we say $a$ and $b$ are *related*/$aRb$.
	- if relation is subset of $A\times A$ then $R$ is a relation *on* $A$
- For any relation $R$ on the set $X$
	- $R$ is *reflexive* if $xRx$ for all $x \in X$
	- $R$ is *symmetric* if $xRy$ implies that $yRx$
	- R is *antisymmetric* if $xRy$ and $yRx$ implies $x=y$
	- R is *transitive* if $xRy$ and $yRz$ implies $xRz$
# Partial Ordering
- If $R$ is a relation on set $X$, $R$ is a *partial ordering* if it is reflexive, anti-symmetric, and transitive
	- Any partial ordering is a *linear/total ordering* if for any elements $x,y\in X$, either $xRy$, $yRx$, or both
# Equivalence Relation
- If $R$ is a relation on set $X$, $R$ is an *equivalence relation* if it is reflexive, symmetric, and transitive
	- $a\sim b$
## Equivalence Classes
- Let $R$ be an equivalence relation on a set $X$. For all $x \in X$, we define the equivalence class of $x$ modulo $R$, or $[x]_{R}$, as $[x]_{R}=\{ y\in X|x\sim y \}$ 
- For any $y\in[x]_{R}$, we call $y$ a *representative element* of $[x]_{R}$