# Basic Terms
- Mathematical claim that has been proves is called
	- *theorem/proposition* if it is a particularly important result
	- *corollary* if it is a statement that immediately follows from a theorem
	- *lemma* if it is a more technical but useful claim
# Mathematical Proof
"An argument in favor of a mathematical statement that will convince the preponderance(most) of knowledgeable mathematicians of the truth of the mathematical statement"
# Mathematical Statement
- A *mathematical statement* is an assertion about mathematical concepts that can be assigned either true or  false
	- ex) $x^3-1=x$ is not mathematical statement, but "there exists $x \in \mathbb{R}$ s.t. $x^3-1=x$" is
## Notation
- Generally use $P,Q,R,\dots$ to represent mathematical statements
- $\sim P$ means not $P$
## Conditional Statements
- The notation $P\implies Q$ can be read as "$P$ implies $Q$"
- This implication is false if $P$ is true and $Q$ is false.
- This implication is true if whenever $P$ is true, $Q$ is also true
- Note this means that if $P$ is never true, then $P\implies Q$ is true
### Converse and Contrapositive
- The converse of $P\implies Q$ is $Q\implies P$
- The contrapositive of $P\implies Q$ is $\sim Q\implies \sim P$
## Biconditional Statements
- A *biconditional statement* is the combination of a conditional statement with its converse: $P\iff Q$, or $P$ if and only if $Q$
- Requires both statements to have the same truth value
#  Open Formulas
- an *open mathematical formula* in variables $x_{1},x_{2},\dots,x_{3}$ is a mathematical expression in which substitution of the variables by specific elements yields a mathematical statement
# Universal Quantifiers
- Let $P(X)$ be a formula in one variable, with universe $U$. Let $X\subseteq U$. Let $Q$ be the statement $(\forall x \in X)P(X)$
- Then $Q$ is true if $P(x)$ is true for all $x \in X$. otherwise $Q$ is false
# Existential Quantifiers
- Let $P(X)$ be a formula in one variable, with universe $U$. Let $X\subseteq U$. Let $Q$ be the statement $(\exists x \in X)P(X)$
- Then $Q$ is true if $P(x)$ is true for at least one $x \in X$. otherwise $Q$ is false
# Proving Universal Statements
- A *universal statement* takes the form:
$$
(\forall x)[H(x)\implies P(x)]
$$
- Direct Proof
	- Assume $H(x)$ and show that $P(x)$ follows
- Contrapositive proof
	- Assume $\sim P(x)$ and show that $\sim H(x)$ follows
- Proof by contradiction
	- Assume that $H(x)$ and $\sim P(x)$ holds, and show that this leads to a logical contradiction.
## Example Proofs
- Prove: An integer is even if and only if it is the sum of two odd integers (Direct Proof)
	- Suppose $n$ is an even integer. Let $n=2m$ where $m\in \mathbb{Z}$ since n is even. Note that $2m=(2m+1)+ (-1)$. $2m+1$ is odd and $-1$ is odd. q.e.d
	- Let $n$ be the sum of two odd integers, say $2m_{1}+1$ and $2m_{2}+1$ where $m_{1},m_{2}\in \mathbb{Z}$. Then $n=2m_{1}+1+2m_{2}+1=2(m_{1}+m_{2})+2=2(m_{1}+m_{2}+1)$. Therefore, $n$ is even. q.e.d
- Prove: Suppose $x$ is an integer. If $x^2$ is even, then $x$ is even (Contrapositive Proof)
	- We are going to prove the contrapositive. Suppose $x$ is odd, then $x=2k+1$ where $k\in \mathbb{Z}$. Then $x^2=(2k+1)^2=4k^2+4k+1=2(2k^2+2k)+1$ and since $2k^2+2k\in \mathbb{Z}$ then $x^2$ is odd. q.e.d
- Prove: There are an infinite amount of prime numbers (Proof by contradiction)
	- We will use a proof by contradiction and assume that $\{ p_{1},p_{2},\dots,p_{n} \}$ is the complete set of prime numbers. Let $n=p_{1}*p_{2}*p_{3}*\dots*p_{n}+1$ , we note that for each $p_{k}$ where $k\in \{ 1,\dots,n \}:p_{k}\not|$ because $p_{k}|p_{1}*p_{2}*p_{3}*\dots*p_{n}$ and $p_{k}\not|1$. Therefore, either $n$ is prime or  there is some prime $p$ that divides $n$ that is not in the set