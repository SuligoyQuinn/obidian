# 1
## a
$$
S(a, b) = \begin{cases}
-1 & a >b \\
p_{1} & A[p_{1}]=t \\
S(a, p_{1}-1) & A[p_{1}]>t \\
p_{2} & A[p_{2}]=t \\
S(p_{1}+1, p_{2}-1) & A[p_{2}]>t \\
S(p_{2}+1,b) & \text{else}
\end{cases}
$$
$$
T(n)=\begin{cases}
c & \text{if }n\leq 1 \\
T\left( \left\lfloor  \frac{n}{3}  \right\rfloor  \right)+d & \text{if }n>1
\end{cases}
$$
$$
T(n)=c+\sum^{\lfloor \log_{3} n \rfloor }_{i=1}d=c+d\lfloor \log_{3}n \rfloor 
$$
## b
### i
$$
T(n) \in O(\log n)
$$
$$
T(n)\in \Omega(\log n)
$$
### ii
$$
T(n)\leq a\log_{2}n \text{ for }n\geq n_{0}
$$
$$
T(n)\geq
$$
### iii
Proof: (by induction on $n$)
Base case: $n=1$
$T(1)=c\leq a\log_{2}(1) = 0$
Inductive hypothesis: Assume $T(k)\leq a\log_{2}(k)$ for $k < n$
Inductive case: $n > 1$
$T(n)=T\left( \left\lfloor  \frac{n}{3}  \right\rfloor \right)+d$, by the inductive hypothesis $T(n)\leq a\log_{2}\left( \left\lfloor  \frac{n}{3}  \right\rfloor \right)$ 

