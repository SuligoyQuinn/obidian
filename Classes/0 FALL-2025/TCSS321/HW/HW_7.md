# 1
Let $n\in \mathbb{Z}\equiv3(\text{mod 7})$, then $n=7k+3$ for some integer $k$. Thus $n^3=(7k+3)^3=343k^3+441k^2+189k+27$. Then we can pull out a $7$, $n^3=7(49k^3+63k^2+27k)+27$ making $n^3\equiv 27(\text{mod }7)$. Note that $27\equiv 6(\text{mod }7)$, making $n^3\equiv 6(\text{mod 7})$.
# 2
For all $n\in \mathbb{Z}$ $n$ is congruent to $0,1,2,3(\text{mod 4})$. If $n\equiv 0(\text{mod 4})$ then $n=4k$ for some integer $k$. Thus $n^4=(4k)^4=256k^4=4(64k^4)\equiv 0(\text{mod 4})$. If $n\equiv 1(\text{mod 4})$ then $n=4k+1$ for some integer $k$. Thus $n^4=(4k+1)^4=256k^4+256k^3+96k^2+16k+1$. Then we can pull out a $4$, $4(64k^4+64k^3+24k^2+4k)+1\equiv 1(\text{mod }4)$. If $n\equiv 2(\text{mod }4)$ then $n=4k+2$ for some integer $k$. Thus $n^4=256k^4+512k^3+384k^2+128k+16$. Then we can pull out a $4$, $4(64k^4+128k^3+96k^2+32k+4)\equiv 0(\text{mod 4})$. If $n\equiv 3(\text{mod 4})$ then $n=4k+3$ for some integer $k$. Thus $n^4=256k^4+768k^3+864k^2+432k+81$. Then we can pull out a $4$, $4(64k^4+192k^3+216k^2+108k)+81\equiv 81(\text{mod }4)$. Note that $81\equiv 1(\text{mod }4)$ making $n^4\equiv 1(\text{mod }4)$. In all cases $n^4$ is congruent to either $0$ or $1$ $(\text{mod }4)$.
# 3
## a
$45=2^0\cdot3^2\cdot 5\cdot 7^0$
$84=2^2\cdot 3\cdot 5^0\cdot 7$
$gcd(45,84)=2^{\text{min(0,2)}}\cdot3^{\text{min(2,1)}}\cdot5^{\text{min(1,0)}}\cdot7^{\text{min(0,1)}}$=$2^0\cdot 3^1\cdot 5^0\cdot 7^0=1\cdot 3\cdot 1\cdot 1=\boxed{3}$
## b
$990=2^1\cdot 3^2\cdot 5^1\cdot 7^0\cdot 11^1$
$1617=2^0\cdot 3^1\cdot 5^0\cdot 7^2\cdot 11^1$
$gcd(990,1617)=2^{\text{min(1,0)}}\cdot3^{\text{min(2,1)}}\cdot5^{\text{min(1,0)}}\cdot7^{\text{min(0,2)}}\cdot 11^{\text{min(1,1)}}=2^0\cdot 3^1\cdot 5^0\cdot 7^0\cdot 11^1=1\cdot 3\cdot 1\cdot 1\cdot 11=\boxed{33}$
# 4
## a

| $r$  | $x$  | $y$  |
| ---- | ---- | ---- |
|      | $89$ | $34$ |
| $21$ | $89$ | $21$ |
| $5$  | $21$ | $5$  |
| $1$  | $5$  | $1$  |
| $0$  | $1$  | $0$  |
$$
\boxed{1}
$$
## b

| $r$   | $x$    | $y$    |
| ----- | ------ | ------ |
|       | $1512$ | $1248$ |
| $264$ | $1248$ | $264$  |
| $192$ | $264$  | $192$  |
| $72$  | $192$  | $72$   |
| $48$  | $72$   | $48$   |
| $24$  | $48$   | $24$   |
| $0$   | $24$   | $0$    |
$$
\boxed{24}
$$
# 5
I feel I have mostly mastered concepts about quantifiers, predicates, and logical statements. And I feel I probably understand prime numbers and modular arithmetic the least, although after last class I think I have a decent grasp on them. I think I understand logical statements the best because I enjoy breaking things down into simpler terms and logical stuff is about as simple as it gets. I'm not really sure why I struggle more with prime numbers and modular arithmetic but I think it's because I'm not sure where they are really used.