# Divisibility
- If $a,b\in \mathbb{Z}$ with $b\neq0$, and $a=mb$ for some integer $m$, then we say that *a is divisible by b* and *b divides a*. We can write the latter as $b|a$
- We say that a natural number other than $1$ is *prime* if its only positive factors are $1$ and itself.
- We say that two integers $a$ and $b$ are *relatively prime* if the greatest factor that they share is $1$
	- every number is relatively prime with $1$
# Integer Combinations
- Given two integers $a$ and $b$, and any other two integers $m$ and $n$, the number $ma+nb$ is called an *integer combination* of $a$ and $b$
	- all possible sums/differences of multiples of $a$ and $b$
- *Proposition 7.1.* if integers $a$ and $b$ are relatively prime, then $a-b$ and $b$ are relatively prime
	- Contrapositive Proof: if $a-b$ and $b$ share a common factor $c$, then $a$ and $b$ share the common factor $c$. Suppose $a-b=nc$ for some $n,c\in \mathbb{Z}$ and $b=mc$ for some $m\in \mathbb{Z}$. And so $nc+ mc=(a-b)+b=a$, which means that $a$ is a multiple of $c$. And so $a$ and $b$ share the common factor $c$. $q.e.d$ 
- *Proposition 7.2.* if integers $a$ and $b$ are relatively prime, then $1$ is an integer combination of $a$ and $b$.
	- We shall argue for a case in which $a$ and $b$ are natural numbers, which can be extended to integers by changing the signs. This allows us to argue by induction on the sum of the integers. The base case for this argument by induction will be $a+b=3$. If $a=0=b$, then $a$ and $b$ are not relatively prime. If $a+b=1$, then $a$ and $b$ are relatively prime and the choice of $m$ and $n$ is obvious. If $a=b=1$ then $a$ and $b$ are relatively prime and again the choice of $m$ and $n$ is obvious. Proof: we may assume that $a>b>0$. We argue by induction on $a+b$. Bases Case: $a+b=3$. Then $a=2$ and $b=1$. So $a-b=1$. Induction step: Assume that the result holds for all pairs of relatively prime natural numbers with sum less than $a+b$. By proposition 7.1, $b$ and $a-b$ are relatively prime. By the induction hypothesis, there are $i,j\in \mathbb{Z}$ such that $i(a-b)+jb=1$ Let $m=i$ and $n=j-i$ Then $ma+nb=1$. By the induction principle the result holds for all relatively prime pairs of natural numbers. $q.e.d$
# Greatest Common Divisor
- Given integers $a,b$ not both $0$, the *greatest common divisor* $gcd(a,b)$ is the largest natural number that divides both $a$ and $b$. We also say that $gcd(0,0)=0$.