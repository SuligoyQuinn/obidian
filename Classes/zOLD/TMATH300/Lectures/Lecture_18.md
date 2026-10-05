# Reminder Complex Numbers
- *complex number* is expression of the form $a+ib$, where $a,b\in \mathbb{R}$. Let $\mathbb{C}=\{ a+ib|a,b\in \mathbb{R} \}$
- Leave $i$ undefined, remove $i$ by representing $a+bi$ as $(a,b)$.
	- Suggests natural bijection between $\mathbb{C}$ and $\mathbb{R}^2$
# Reminder Polar Complex Numbers
- Can convert $(r,\theta)$ to $(x,y)$ by noting that $x=r\cos \theta$ and that $y=r\sin \theta$.
- Implies that $a+bi=r(\cos \theta+i\sin \theta)$ abbreviated as $rCis(\theta)$
	- Example $r_{1}Cis(\theta_{1})\cdot r_{2}Cis(\theta_{2})$
		$r_{1}Cos\theta_{1}+ir_{1}Sin \theta_{1}\cdot r_{2}Cos\theta_{2}+ir_{2}Sin \theta_{2}=$ 
- $$r_{1}r_{2}Cos\theta_{1}Cos\theta_{2}+r_{1}ir_{2}Cos\theta_{1}Sin \theta_{2}+ir_{1}r_{2}Sin\theta_{1}Cos\theta_{2}+ir_{1}ir_{2}Sin \theta_{1}Sin \theta_{2}$$$$
r_{1}r_{2}Cos\theta_{1}Cos\theta_{2}-r_{1}r_{2}Sin \theta_{1}Sin \theta_{2}+i(r_{1}r_{2}Cos\theta_{1}Sin \theta_{2}+r_{1}r_{2}Sin\theta_{1}Cos\theta_{2})
$$
$$
r_{1}r_{2}Cos(\theta_{1}+\theta_{2})+ir_{1}r_{2}Sin(\theta_{1}+\theta_{2})
$$
- Magnitudes multiply, angles add
# De Moivre's Theorem
- *Theorem 9.20* Let $z=rCis(\theta)$ be a non-zero complex number, and let $n\in \mathbb{Z}$. Then $z^n=r^nCis(n\theta)$
- $z^4=\left\{  (1,0),(1,\pi),\left( 1, \frac{\pi}{2} \right),\left( 1, \frac{3\pi}{2} \right)  \right\}$
- $z^5=\left\{  1,Cis\left( \frac{2\pi}{5} \right),Cis\left( \frac{4\pi}{5} \right),\left( Cis\left( \frac{6\pi}{5} \right) \right)  \right\}$
# Roots for $\mathbb{C}$
- *Theorem 9.22.* Let $z=rCis(\theta)$ be a non-zero complex number and let $n$ be an integer greater than $1$. Then there are exactly $n$ complex solutions to the equation $w^n$=z. They are
	- $\left\{  r^\frac{1}{n}Cis\left( \frac{\theta}{n}+\frac{2k\pi}{n} \right)|k=0,1,\dots,n-1  \right\}$
# Primitive Roots of Unity
- A $n$th *root of unity* is a $\omega \in \mathbb{C}$ such that $\omega^n=1$
	- There are exactly $n$ $n$th roots of unity
- A *primitive root of unity* is a number $\omega$ such that $\{ 1,\omega,\omega^2,\dots,\omega^{n-1} \}$ constitutes all the $n$th roots of unity of 1
	- $\{ i,-1,-i,1 \}$ and $\{ -i,-1,i,1 \}$ means $i$ and $-i$ are primitive 4th roots of unity
	- Connection to relatively prime numbers
# True Triangle Inequality
- *Lemma 9.36.* Let $z_{1},z_{2}$ be complex numbers, then $|z_{1}+z_{2}|\leq|z_{1}|+|z_{2}|$
# Fundamental Theorem of Algebra
- *Theorem 9.44.* Let $p \in \mathbb{C}[z]$ be a polynomial of degree $N\geq1$. Then $p$ can be factored as $p(x)=c(z-a_{1})\dots(z-a_{N})$
- For complex numbers $c,a_{1},\dots,a_{N}$. This factoring is unique up to order.