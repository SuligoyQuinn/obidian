# 1
## a
1
$$
\Theta(n^2)
$$
2
$$
\Theta(n^2)
$$
3
$$
\Theta(n\log(n))
$$
4
$$
\Theta(n)
$$
## b
$a$: loop conditional
$b$: appending
$c$: linear search
$d$: initialization
$$
f_{1}(n)=d+\sum^n_{i=1}(a+c(i-1)+b)
$$
$a$: loop conditional
$b$: sorted insertion
$c$: binary search
$d$: initialization
$$
f_{2}(n)=d+\sum^n_{i=1}(a+c\log(i-1)+b(i-1))
$$
$a$: loop conditional
$b$: insertion
$c$: contains
$d$: initialization
$$
f_{3}(n)=d+\sum^n_{i=1}(a+c\log(i-1)+b\log(i-1))
$$
$a$: loop conditional
$b$: insertion 
$c$: contains
$d$: initialization
$$
f_{4}(n)=d+\sum^n_{i=1}(a+c+b)
$$
## c
$$
f_{1}(n)=d+\sum^n_{i=1}(a+c(i-1)+b)
$$
$$
f_{1}(n)=d+\sum^n_{i=1}a+\sum^n_{i=1}b+c\left( \sum^n_{i=1}i-\sum^n_{i=1}1 \right)
$$
$$
f_{1}(n)=d+na+nb+c\left( \frac{n(n+1)}{2}-n\right)
$$
$$
\boxed{f_{1}(n)=d+n\left( a+b+c\left( \frac{n+1}{2}-1 \right) \right)}
$$
---
$$
f_{2}(n)=d+\sum^n_{i=1}(a+c\log(i-1)+b(i-1))
$$
$$
f_{2}(n)=d+\sum^n_{i=1}a+b\left( \sum^n_{i=1}i-\sum^n_{i=1}1 \right)+c\sum^n_{i=1}\log(i-1)
$$
$$
\sum^n_{i=1}\log(i-1)\leq \sum^n_{i=1}\log(n-1)
$$
$$
\sum^n_{i=1}\log(i-1)\leq(n-1)\log(n-1)=O(n\log n)
$$
$$
\sum^n_{i=1}\log(i-1)\geq \sum^n_{i=\left\lceil  \frac{n}{2}  \right\rceil }\log(i-1)
$$
$$
\sum^n_{i=1}\log(i-1)\leq \frac{n}{2}\log\left( \frac{n}{2} \right)=\Omega(n\log n)
$$
$$
f_{2}(n)=d+na+b\left( \frac{n(n+1)}{2}-n \right)+c\Theta(n\log n)
$$
$$
\boxed{f_{2}(n)=d+n\left( a+b\left(\frac{n+1}{2}-1\right) \right)+c\Theta(n\log n)}
$$
---
$$
f_{3}(n)=d+\sum^n_{i=1}(a+c\log(i-1)+b\log(i-1))
$$
$$
f_{3}(n)=d+\sum^n_{i=1}a+b\sum^n_{i=1}\log(i-1)+c\sum^n_{i=1}\log(i-1)
$$
$$
\boxed{f_{3}(n)=d+na+b\Theta(n\log n)+c\Theta(n\log n)}
$$
---
$$
f_{4}(n)=d+\sum^n_{i=1}(a+c+b)
$$
$$
f_{4}(n)=d+\sum^n_{i=1}a+\sum^n_{i=1}b+\sum^n_{i=1}c
$$
$$
f_{4}(n)=d+na+nb+nc
$$
$$
\boxed{f_{4}(n)=d+n(a+b+c)}
$$
# 2
$4<3<1<2$
$4$ is the fastest algorithm
# 3
$$
f_{1}(500000)=1+500000\left( 1+1+1\left( \frac{500000+1}{2}-1 \right) \right)
$$
$$
\boxed{f_{1}(500000)=1.2500075\cdot10^{11}}
$$
---
$$
f_{2}(500000)=1+500000\left( 1+1\left(\frac{500000+1}{2}-1\right) \right)+1\Theta(500000\log 500000)
$$
$$
\boxed{f_{2}(500000)=1.2500309949\cdot 10^{11}}
$$
---
$$
f_{3}(500000)=1+500000(1)+1\Theta(500000\log 500000)+1\Theta(500000\log 500000)
$$
$$
\boxed{f_{3}(500000)\approx 6198971}
$$
---
$$
f_{4}(500000)=1+500000(1+1+1)
$$
$$
\boxed{f_{4}(500000)=1500001}
$$