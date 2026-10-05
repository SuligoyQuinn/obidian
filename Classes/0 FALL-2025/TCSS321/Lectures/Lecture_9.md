# Rules of Inference
- Modus Tollens
$$
\neg q
$$
$$
p\implies q
$$
---
$$
\therefore  \neg p
$$
- Hypothetical syllogism
$$
p\implies q
$$
$$
q\implies r
$$
---
$$
\therefore  p\implies r
$$
- Resolution
$$
p\lor q
$$
$$
\neg p\lor r
$$
---
$$
\therefore  q\lor r
$$
## For Quantified Statements
- Universal Instantiation
$$
\forall xP(x)
$$
---
$$
\therefore  P(c)
$$
- Universal generalization (for arbitrary $c$)
$$
P(c)
$$
---
$$
\therefore  \forall xP(x)
$$
- Existential Instantiation (for some element $c$)
$$
\exists xP(x)
$$
---
$$
\therefore P(c)
$$
- existential generalization
$$
P(c)
$$
---
$$
\therefore  \exists xP(x)
$$
# Proofs
- Direct Proof
	- Ex) If $n$ is an odd integer, then $n^2$
	- Let $n$ be an odd integer, then $n=2k+1$ for some integer $k$. W.M.S.T $n^2=(2k+1)^2=4k^2+4k+1$. Then $4k^2+4k+1=2(2k^2+2k)+1$. Because $2k^2+2k$ is an integer then the equation is in the form $2k+1$ for some integer $k$ making $n^2$ odd.