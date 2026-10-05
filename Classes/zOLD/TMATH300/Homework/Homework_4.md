# 4.1
Base case: let $n=1$, we note that $7^1-4=7-4=3$, and $3|3$. 
Induction step: start with $7^{n+1}-4$ and add and subtract $7$ from both sides, $7^{n+1}-4+7-7=7(7^n-1)+3$. Note that as $7^n+1$ is divisible by $3$ then $7^n+1=3k$ for some $k\in \mathbb{N}$, in the previous equation this means $$7(7^n-1)+3=7(3k)+3=21k+3=3(7k+1)$$
As $7^{n+1}-1=3(7k+2)$ this means $7^{n+1}-1|3$ if $7^n-1|3$. Which through the principle of induction implies 3 divides $7^n-4$ for every $n\in \mathbb{N}^+$
# 4.4
Base Case: let $n=1$, meaning $(1+x)^1\geq 1+1x\implies1+x\geq 1+x$, thus the inequality holds for $n=1$.
Induction Step: let $(1+x)^n\geq 1+ nx$,(W.M.S.T $(1+x)^{n+1}\geq1+nx+x$) then multiply both sides, $(1+x)(1+x)^n\geq(1+nx)(1+x)$. We can rewrite the equality to get $(1+x)^{n+1}\geq1+n+nx+nx^2$. Note that $nx^2$ will always be positive, meaning $1+nx+x > 1+nx+x+nx^2$ . Which implies $(1+x)^{n+1}\geq1+nx+x$
# 4.7
Base Case: Let $n=0,k=0$. Note that $\binom{0}{0}=1$ and $\frac{0!}{0!0!}=\frac{1}{1\cdot1}=1$
Induction Step: We want to prove $\binom{n}{k}=\frac{n!}{k!(n-k)!}$ using $\binom{n}{k}=\binom{n-1}{k}+\binom{n-1}{k-1}$. Using the induction hypothesis on the right hand side we get $\binom{n-1}{k}+\binom{n-1}{k-1}=\frac{(n-1)!}{k!(n-1-k)!}+\frac{(n-1)!}{(k-1)!(n-k)!}$. In order to get a common denominator for the fraction note that $k!= k\cdot(k-1)!$ and $(n-1-k)!=(n-k-1)!=\frac{(n-k)!}{n-k}$. Multiplying both fraction to get a common base and combining, we get $\frac{(n-1)!}{k!(n-k)!}\cdot n=\frac{n!}{k!(n-k)!}$ which matches the formula for $\binom{n}{k}$.
# 4.11
We will use a proof by contradiction, assume there is a strictly decreasing infinite series, that is $a_{1}>a_{2}>\dots>a_n$ which implies $a_{n}>a_{n+1}$. As $0$ is the smallest natural number this series must eventually have $0$ as the last element, which is a contradiction as it is supposed to be infinite. This proves the Principle of Descent.
# 4.20
a) Let $f(0)=k$, because $f(x+y)=f(x)+f(y)$, then $f(0+0)=f(0)+f(0)\implies k=k+k$. The only way this can be possible is if $k=0$.
b) let $n\in \mathbb{R}$, note that $n=\sum^n_{i=0}1$, thus $f(n)$ can be written as $f(1)+f(1)$ $n$ times or $nf(1)$