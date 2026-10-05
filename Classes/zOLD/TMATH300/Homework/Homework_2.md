# 2.4
Let $x=\{ a,b \}$.  Then $xRx$ is true as $ab=ba$. This makes $X$ reflexive.
Let $x=\{ a,b \},y=\{ c,d \}$.  Suppose $xRy$. This means $ad=bc$, which implies $da=cb$. This makes $yRx$, showing that $R$ is symmetric
Let $x=\{ a,b \},y=\{ c,d \},z=\{ e,f \}$. Suppose $xRy$ and $yRz$. This means $ad=bc$ and $cf=de$, then through algebra $(ad)(cf)=(bc)(de)\implies adcf=bcde\implies af=be$. Which makes $xRz$, this implies $R$ is transitive
As $R$ is reflexive, symmetric, and transitive, it is an equivalence relation.
# 2.9
I:
Reflexive, Symmetric
II:
Symmetric
III:
Reflexive, Antisymmetric, Transitive
IV:
Reflexive, Symmetric, Transitive
# 2.19
Let $n=x^2+y^2+z^2$ where $x,y,z\in \mathbb{N}$. Note that $\mathbb{N}^2_{8}=\{0,1,4,1,0,1,4,1  \}$, this means that $n$ mod $8$ can only be written as the sum of $0,1,4$ 3 times. The only number that does not come out of this sequence is $7$, this means you cannot get $7$ mod $8$ from a sum of three squares. As there are infinite natural numbers congruent to $7$ mod $8$ this means the set $\{n\in N:n\equiv 7mod 8\}$ is infinite. q.e.d

# 2.22

Let $W=\{ 0,1,2 \}, Z=\{ 0,1 \}, f:W\to \lceil 2 \rceil=\{ (0,1),(1,0),(2,1) \},g:Z\to \lceil 2 \rceil=\{ (0,1),(1,0)\}$. In this scenario $f$ is related to $g$ as $Dom(g)\subseteq Dom(f)$ and $g=f|_{Dom(g)}$. We can see that while $fRg$ is true, $g$ not related to $f$, this means $R$ is not symmetric thus $R$ is not an equivalence relation. We can also see that $fRf$ as $Dom(f)\subseteq Dom(f)$. This is true for any function, as the domain will always be equal to itself, making $R$ reflexive
Suppose $fRg$ and $gRf$, this means $Dom(g)\subseteq Dom(f), Dom(f)\subseteq Dom(g), g=f|_{Dom(g)},$ and $f=g|_{Dom(f)}$. This means that $Dom(g)=Dom(f)$ and the functions agree on that domain, this implies $f=g$ making $R$ anti-symmetric
Suppose $fRg$ and $gRh$, this means $Dom(g)\subseteq Dom(f)$ and $Dom(h)\subseteq Dom(g)$ which implies $Dom(h)\subseteq Dom(f)$. Also $h=g|_{Dom(h)}=f|_{Dom(h)}$. This makes $R$ transitive
As $R$ is reflexive, antisymmetric, and transitive, $R$ is a partial ordering.
# 2.23
For every $f\in X$ $fRf$ as $f^{-1}(1)\subseteq f^{-1}(1)$. This makes $R$ reflexive.
Let $f(n)=1$ if $n=0$, otherwise $0$, and $g(n)=1$ for all $n\in \mathbb{N}$, then $f^{-1}(1)=\{ 0 \}$ and $g^{-1}(1)=\{ \mathbb{N}\}$. Because $\{ 0 \}\subseteq \mathbb{N}, fRg$ however $\mathbb{N}\not\subseteq \{ 0 \}$ meaning $g$ is not related to $f$. Through proof by contradiction this makes $R$ not symmetric 
Suppose $fRg$ and $gRf$, this means $f^{-1}(1)\subseteq g^{-1}(1)$ and $g^{-1}(1)\subseteq f^{-1}(1)$, which implies $f^{-1}(1)=g^{-1}(1)$. This means $g(n)=1$ iff $f(n)$. Because $f$ and $g$ are binary sequences if $f(n)\neq 1$, then $f(n)=0$,  which also implies $g(n)=0$. This means $f(n)=g(n)$ for all $n\in \mathbb{N}$. This makes $R$ antisymmetric.
Suppose $fRg$ and $gRh$, this means $f^{-1}(1)\subseteq g^{-1}(1)$ and $g^{-1}(1)\subseteq h^{-1}(1)$ this implies $f^{-1}(1)\subseteq h^{-1}(1)$, which means $fRh$. This makes $R$ transitive.
As $R$ is reflexive, antisymmetric, and transitive, $R$ is a partial ordering and not an equivalence relation.