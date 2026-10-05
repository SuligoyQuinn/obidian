# Dedekind Cut
- A *Dedekind cut* $L$ is a nonempty proper subset of $\mathbb{Q}$ that has no maximal element and satisfies
	- $(\forall a,b\in \mathbb{Q})[a\in L\wedge b<a]\implies[b\in L]$
	- Cuts number line to the left
- Let $R=\mathbb{Q}\textbackslash L$
	- Right part of cut
	- $R$ is nonempty as $L$ is a proper subset of $\mathbb{Q}$, therefor $L$ and $R$ partition $\mathbb{Q}$
# Dedekind Cut and the Rationales
- Let $D$ be the set of Dedekind cuts. We can create an injection $i:\mathbb{Q}\to D$ where
	- $i(a)=\{ b\in \mathbb{Q}|b<a \}$
- Can define addition, multiplication, and linear ordering on $D$
# Dedekind Cut and the Reals
- Define the *real numbers* $\mathbb{R}$ as $D$ with the addition, multiplication, and $\leq$ as previously defined
# Least Upper Bound Property
- Let $X\subset D$. We say that $X$ is *bounded above* if $\exists M\in D$ such that $(\forall \\x\in X)x\leq M$ and $M$ is an *upper bound* for $X$.
- Let $X\subset D$ be bounded above. Suppose $M$ is an upper bound for $X$ such that for any upper bound $N$ for $X$, $M\leq N$. Then the number $M$ is called the *least upper bound* for $X$.
- *Theorem 8.3.* if $X$ is a non-empty subset of $D$ and is bounded above, then $X$ has a least upper bound(or *supremum*)
# New Cut
- Let $T=\bigcup_{L\in D}[L^2<2].$
	- Is non-empty
	- Is bounded above
	- Does have a supremum
	- Supremum cannot be rational
# Real Sequences
- A *real sequence* is a function $a:\mathbb{N}\to \mathbb{R}$. We usually designate the term $a(n)$ as $a_{n}$ and the sequence as $\langle a_{n}\rangle$. 
- Let $\langle a_{n}|n\in \mathbb{N} \rangle$ be a sequence and $f\in \mathbb{N}^\mathbb{N}$ be a strictly increasing sequence of natural numbers. Then
	- $\langle a_{f(n)}|n\in \mathbb{N} \rangle$ is a subsequence of $\langle a_{n}|n\in \mathbb{N} \rangle$
# Sequence Convergence
- The sequence $\langle a_{n} \rangle$ tends to the limit $L$ as $n$ goes to infinity, written $\lim_{ n \to \infty }a_{n}=L$ if for every $\epsilon>0$ there exists $N\in \mathbb{N}$ such that $(\forall n\in \mathbb{N})n>N\implies|a_{n}-L|<\epsilon$
- Ex) Prove that the sequence $a_{n}=\frac{1}{n}$ converges to 0
	- Let $\epsilon>0$. Then choose $N\in \mathbb{N}$ s.t. $N>\frac{1}{\epsilon}$, then $\forall n>N$, we know that $\frac{1}{n}< \frac{1}{N}< \epsilon$. Thus, since $\frac{1}{n}$ is always positive, we have that $(|a_{n}|<\epsilon)$ $\forall n>N$ and so $a_{n}\to 0$ as $n\to \infty$
# The Bolzano-Weierstrass Theorem
- *Theorem 6.8.* Let $[b,c]$ be a closed bounded interval of real numbers and $s=\langle a_{n}|n\in \mathbb{N} \rangle$ be a sequence of real numbers such that $(\forall n\in \mathbb{N})a_{n}\in[b,c]$. Then $\langle a_{n} \rangle$ has a convergent subsequence with limit in $[b,c]$ 