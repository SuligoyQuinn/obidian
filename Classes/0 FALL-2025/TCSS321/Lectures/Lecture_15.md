# Functions in Algorithms
- $1$
- $\log n$
- $n$
- $n\log n$
- $n^2$
- $2^n$
- $n2^n$
- $n!$
- $n^n$
# Big Omega
- $f(n)$ is $\Omega(g(n))$ if there exists constants $c$ and $k$ such that $f(n)\geq cg(n)$ for all $n>k$
# Big Theta
- $f(n)$ is $\theta(g(n))$ if $f(n)$ is $O(g(n))$ and $f(n)$ is $\Omega(g(n))$
# Divisibility
- For integers $a$ and $b$, where $a\neq0$, $a$ divides $b$ if there is an integer $c$ such that $b=ac$. $a$ is a factor of $b$, $b$ is a multiple of $a$, $b$ is divisible by $a$
- Denoted $a|b$
## Theorem 1
- Let $a,b,$ and $c$ be integers where $a\neq 0$.
1) if $a|b$ and $a|c$, then $a|(b+c)$
2) if $a|b$, then $a|bc$ for all $c\in \mathbb{Z}$
3) if $a|b$ and $b|c$, then $a|c$
## Theorem 2 Division Algorithm
- Let $a$ be an integer and $d$ a positive integer. Then there exist unique integers $q$ and $r$, with $0\leq r< d$. Such that $a=dq+r$
	- $a$ is the dividend
	- $d$ is the divisor
	- $q$ is the quotient
	- $r$ is the remainder
	- $q=a$ div $d$
	- $r=a$ mod $d$
- If $a$ and $b$ are integers and $m$ is a positive integer, then $a$ is congruent to $b$ modulo $m$ if $m|a-b$. Denoted $a\equiv b(\text{mod }m)$
## Theorem 4
- Let $m$ be a positive integer. The integers $a$ and $b$ are congruent modulo $m$ iff there is an integer $k$ such that $a=b+km$