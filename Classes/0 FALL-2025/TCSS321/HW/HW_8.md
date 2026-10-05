Quinn Suligoy
# 1
The proof is by induction on $n$. Let $P(n)$ be the statement $a_{n}\geq 2\varphi^n$. Basis steps: $n=0$ then $a_{0}=2\geq 2\varphi^0=2$. $n=1$ then $a_{1}=4\geq2\varphi^1=1+\sqrt{ 5 }$. $n=2$ then $a_{2}=6\geq 2\varphi^2=2(1+\varphi)=3+\sqrt{ 5 }$. Induction Hypothesis: Suppose that for all $1\leq h\leq k$ for some fixed $k\geq 2$, $P(h)$ is true. Induction Step: We must show that $P(k+1)$ is true, that is $a_{k+1}\geq 2\varphi^{k+1}$. By the definition of the recurrence equation  $a_{k+1}=a_{k}+a_{k-1}+a_{k-2}$. By the induction hypothesis $a_{k}\geq 2\varphi^k$, $a_{k-1}\geq 2\varphi^{k-1}$, and $a_{k-2}\geq 2\varphi^{k-2}$. Thus $a_{k+1}\geq 2\varphi^k+2\varphi^{k-1}+2\varphi^{k-2}=2\varphi^{k-2}(\varphi^2+\varphi+1)=2\varphi^{k-2}\cdot 2\varphi^2=4\varphi^k$. Note that because $\varphi \approx 1.618$, $4\varphi^k\geq 2\varphi^{k+1}$. Thus $a_{k+1}>2\varphi^{k+1}$. 
Q.E.D
# 2
The proof is by induction on $n$. Let $P(n)$ be the statement $3|n^3+2n$. Basis step, consider $n=0$, that is $3|0^3+2\cdot 0 = 3|0$ which is true. Induction Hypothesis: Now suppose $P(n)$ is true for some fixed $n\geq 1$, that is $3|n^3+2n$. Induction Step: We must show that $P(n+1)$, that is $3|(n+1)^3+2(n+1)$. This simplifies to $3|n^3+3n^2+3n+1+2n+2=3|n^3+3n^2+5n+3$. We can pull $n^3+2n$ and $3$ out to get $3|3(n^2+n+1)+(n^3+2n)$. Note that by the induction hypothesis $n^3+2n$ is divisible by $3$ therefore we only need to show that $3(n^2+n+1)$ is divisible by $3$. $3(n^2+n+1)\equiv 0(\text{mod }3)$, by the definition of divides, this makes $3(n^2+n+1)$ divisible by $3$. Meaning $P(n+1)$ is true. 
Q.E.D
# 3
## a
$R=\{ (4,6),(5,7),(6,8) \}$
## b
$\begin{bmatrix}X\ 4\ 5\ 6\ 7\ 8 \\ 4\ 0\ 0\ 1\ 0\ 0 \\ 5\ 0\ 0\ 0\ 1\ 0 \\ 6\ 0\ 0\ 0\ 0\ 1 \\ 7\ 0\ 0\ 0\ 0\ 0 \\ 8\ 0\ 0\ 0\ 0\ 0\end{bmatrix}$
## c
No, consider $(4,6)\in R$ and $(6,8)\in R$, however $8\neq 4+2$ meaning $(4,8)\not\in R$.
## d
Yes, consider $\forall x(x,y)\in R$ then $y=x+2$ meaning $y$ is not related to $x$. Thus $(x,y)\in R$ and $(y,x)\in R$ is impossible.
# 4
## a
No, consider $(2,3)\in R$ and $(3,4)\in R$, however $gcd(2,4)\neq 1$ thus $2$ is not related to $4$.
## b
Yes, $gcd(a,b)=gcd(b,a)$
## c
No, $gcd(a,a)=a$
