# Sequence
- A *sequence* is a function from a set of integers to a set $S$.
- We say $a_{n}$ to denote the image of $n$.
- $a_{n}$ is a term in the sequence
## Geometric Progression
- A *geometric progression* is a sequence of the form $a,a*r,a*r^2,a*r^3,\dots$ where $a,r\in \mathbb{R}$
- $a$ is the initial term
- $r$ is the common ratio
## Arithmetic Progression
- A *arithmetic progression* is a sequence of the form $a, a+d, a+2d, a+3d,\dots$ where $a,d\in \mathbb{R}$
- $d$ is the common difference
# Recurrence Relation
- A *recurrence relation* for a sequence $\{ a_{n} \}$ is an equation that expresses $a_{n}$ in terms of one or more previous terms in the sequence
- ex) $a_{n}=a_{n-1} +5$, $a_{0}=0$
	- $a_{0}$ is the initial condition
## Backwards Substitution
- ex) $a_{0}=1$, $a_{n}=2a_{n-1}$
Imagine $n$ is large then we can write $a_{n}=2a_{n-1}=2(2(a_{n-2}))=2(2(2(a_{n-3})))$ repeating this $k$ times we get $2^k(a_{n-k})$. Then set $k$ to a value such that we reach an initial condition. Let $k=n$ $2^n(a_{n-n})=2^n(a_{0})=2^n$.