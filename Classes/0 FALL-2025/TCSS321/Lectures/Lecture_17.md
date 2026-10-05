# Greatest Common Divisor
- Let $a$ and $b$ be integers, not both $0$. The largest integer $d$ such that $d|a$ and $d|b$ is called the greatest common divisor of $a$ and $b$
- Integers $a$ and $b$ are *relatively prime* if $gcd(a,b)=1$
## Lemma
- Let $a=bq+r$, where $a,b,q,r\in \mathbb{Z}$. Then $gcd(a,b)=gcd(b,r)$
## gcd algorithm
```java
gcd(a,b)
	x <- a
	y <- b
	while y != 0
		r <- x mod y
		x <- y
		y <- r
	return x
```

# Least Common Multiple
- Let $a$ and $b$ be positive integers. The smallest integer $n$ such that $a|n$ and $b|n$ is called the least common multiple