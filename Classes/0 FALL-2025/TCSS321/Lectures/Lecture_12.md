# Summations
- suppose you have a sub sequence $a_{1}, a_{m+1},\dots,a_{n}$ from the sequence $\{ a_{n} \}$ 
- The sum of these terms is denoted $\sum^n_{j=m}a_{j}$ or $\sum_{m\leq j\leq n}a_{j}$ or $\sum_{j\in \{ m,m+1,\dots,n \}}a_{j}$
	- $m$ is the lower limit
	- $n$ is the upper limit
	- $j$ is the index of summation
## Changing Limits
$$
\sum^n_{j=m}f(j)=\sum_{j=0}^{n-m}f(j+m)
$$
## Common Sums
$$
\sum^n_{i=1}i=\frac{n(n+1)}{2}
$$
- Where $n\geq m$
$$
\sum^n_{i=m}i=\frac{(n+m)(n-m+1)}{2}
$$
- Where $k$ is constant
$$
\sum^n_{i=m}k=k(n-m+1)
$$
$$
\sum^n_{i=m}(f(i)+g(i))=\sum^n_{i=m}f(i)+\sum^n_{i=m}g(i)
$$
## Sum of Geometric Progression
- Theorem: $a,r\in \mathbb{R}$ and $r\neq 1$ then
$$
\sum^n_{j=0}ar^j=\frac{ar^{n+1}-a}{r-1}
$$
- Proof
If $r=1$, then $\sum^n_{j=0}ar^j=\sum^n_{j=0}a=(n+1)a$. If $r\neq 1$ then let $S_{n}=\sum^n_{j=0}ar^j$. Then $rS_{n}=r\sum^n_{j=0}ar^j=\sum^n_{j=0}ar^{j+1}=\sum^{n+1}_{j=1}ar^j$. Pulling out the last term then gives us $ar^{n+1}+\sum^n_{j=0}ar^j-ar^0$. Then $rS_{n}=S_{n}+ar^{n+1}-a$ or $rS_{n}-S_{n}=ar^{n+1}-a$. Factoring out $S_{n}$ gives us $(r-1)S_{n}=ar^{n+1}-a$ or $S_{n}=\frac{ar^{n+1}-a}{r-1}$ 
- Helpful form
$$
\sum^n_{i=0}2^i=2^{n+1}-1
$$
## Double Summations
$$
\sum^n_{i=1}\sum^n_{j=1}(i+j)=\sum^n_{i=1}\left( \sum^n_{j=1}i+\sum^n_{j=1}j \right)
$$
$$
=\sum^n_{i=1}\left( ni+\frac{n(m+1)}{2} \right)=\sum^n_{i=1}ni+\sum^n_{i=1} \frac{n(m+1)}{2}
$$
$$
=n\sum^n_{i=1}i+(n-1+1)\left( \frac{n(n+1)}{2} \right)=n \frac{n(n+1)}{2}+n\left( \frac{n(n+1)}{2} \right)
$$
$$
=2\left( n \frac{n(n+1)}{2} \right)=\boxed{n^2(n+1)}
$$
# Solving Recurrence Equations
$a_{n}=3a_{n-1}+2$, $a_{0}=1$
$$
a_{n}=3a_{n-1}+2=3(3a_{n-2}+2)+2
$$
$$
=3^2a_{n-2}+3\cdot 2+2=3^2(3a_{n-3}+2)+3\cdot2+2
$$
$$
3^3a_{n-3}+3^2\cdot 2+3\cdot 2+2=3^3(3a_{n-4}+2)+3^2\cdot 2+3\cdot 2+2
$$
$$
3^4a_{n-4}+3^3\cdot 2+3^2\cdot 2+3\cdot 2+2
$$
as we substitute $k$ times we get the equation
$$
3^ka_{n-k}+2\sum^{k-1}_{i=0}3^i
$$
Let $k=n$
$$
3^na_{0}+2\sum^{n-1}_{i=0}3^i
$$
$$
3^n+2\left( \frac{3^n-1}{2} \right)
$$
$$
3^n+3^n-1
$$
$$
2\cdot3^n-1
$$

