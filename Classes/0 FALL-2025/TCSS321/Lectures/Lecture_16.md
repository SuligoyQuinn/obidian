# Modular Arithmetic
## Theorem 5
- Let $m\in \mathbb{Z}^+$, If $a\equiv b(\text{mod }m)$ and $c\equiv d(\text{mod }m)$, then $(a+c)\equiv(b+d)(\text{mod }m)$ and $(a\cdot c)\equiv(b\cdot d)(\text{mod }m)$.
## Homework 7 help
- If $n\in \mathbb{Z}$ then $n^2\equiv 0(\text{mod }3)$ or $n^2\equiv 1(\text{mod 3})$
Proof by contradiction
Assume $n^2\equiv 2(\text{mod 3})$ and $n\in \mathbb{Z}$, by definition of modulo $3|n^2-2$. By definition of divides $n^2-2=3k$ for some $k\in \mathbb{Z}$. Then $n=\sqrt{ 3k+2 }$.
# Integer Representations
- binary: the only digits are $0$ and $1$.
	- $(10110)_{2}$
# Prime Number
- Any number is prime if it is not $1$ and its only positive factors are $1$ and itself.
- Any non-prime number greater than $1$ is called a composite number
## Theorem 1
- Any integer greater than $1$ can be written either as a prime number, or as a product of prime numbers in increasing order.
	- $75=3\cdot 5\cdot 5=3^1\cdot 5^2$
## Theorem 2
- If $n$ is a composite number, then $n$ has a prime factor that is less than or equal to $\sqrt{ n }$.