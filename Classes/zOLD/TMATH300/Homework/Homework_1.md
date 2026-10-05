# 1.2
I:
Let $a\in(X\cup Y)^c$ , then $a \not\in X$ and $a \not\in Y$, so $a\in X^c\cap Y^c$. Let $a\in X^c\cap Y^c$, then $a\not\in X$ and $a\not\in Y$, so $a\in(X\cup Y)^c$
II:
Let $a\in(X\cap Y)^c$, then $a\not\in X$ or $a\not\in Y$, so $a\in X^c\cup Y^c$. Let $a\in X^c\cup Y^c$, then $a\not\in X$ or $a\not\in Y$, so $a\in(X\cap Y)^c$
# 1.15
Let triangle $T\in X$ with sides $a$, $b$, and $c$, and side lengths $|a|=|b|>|c|$. Then $f(T)$ is equal to both $a$ and $b$. making $f$ not a function on set $X$. 
Let triangle $T\in Y$ with legs $a$ and $b$, and hypotenuse $c$. because of right triangle properties, $c$ will always be the longest side length, meaning $f(T)=c$. Making $f$ a function on set $Y$
Let triangle $T\in Z$ with sides $a$, $b$, and $c$. Non-isosceles triangle means $|a| \neq|b|\neq|c|$, making $f(T)$ only return $1$ value. Making $f$ a function on set $Z$
$g$ will always be a function on all sets as even on an equilateral triangle $T$ with sides $|a|=|b|=|c|$, $g(T)=|a|=|b|=|c|$. Only returning one value, making $g$ a function.
$Z^c\in X$ is the set of all isosceles triangles, $Y\cap Z^c$ is the set of all right angled isosceles triangles

# 1.16
I:
$\mathbb{R}$ and $\mathbb{R}$
II:
$(-10,10)$ and $(-10,10)$
III:
$(-10,10)$ and $[-10,10]$
IV:
$(-10,10)$ and $[-10,10]$
V:
$(-10,10)$ and $(-10,10)$
VI:
$0$ and $0$
# 1.20
Assume $g\circ f$  is injective and $f$ is not injective, meaning $f(a)=f(b)$ and $a\neq b$. This would mean that $g(f(a))=g(f(b))$ while $a\neq b$ making $g\circ f$ not injective. This contradiction means that if $g\circ f$ is injective then $f$ must be injective.
Let $X = \{ 1,2 \}, Y=\{ a,b,c \}, Z=\{ 0,1 \}$.  And $f:X\to Y = \{ (1,a),(2,b) \}$ and $g:Y\to Z=\{ (a,0),(b,1),(c,0) \}$. This makes $f$ injective while $g$ not injective. However $g\circ f:X\to Z=\{ (1,0),(2,1) \}$ making $g\circ f$ injective. 

# 1.21
Assume $f: X\to Y$ is surjective and $g:Y\to Z$ is surjective. This means for every $z\in Z$ there exists a number $y\in Y$ such that $g(y)=z$ and for every $y\in Y$ there exists a number $x\in X$ such that $f(x)=y$. Thus for every $z\in Z$ there exists a number $x \in X$ such that $g\circ f(x)=z$, making $g\circ f:X\to Y$ surjective.
Let $X=\{ 1,2 \},Y=\{ a,b,c \},Z=\{ 0,1 \}$. And $f:X\to Y=\{ (1,a),(2,b) \}$ and $g:Y\to Z=\{ (a,0),(b,1) \}$. This makes $f$ not surjective as there is no number $x \in X$ for which $f(x)=c$. However for every $z\in Z$ there exists an $x \in X$ such that $g\circ f(x)=z$ making $g\circ f$ surjective.
