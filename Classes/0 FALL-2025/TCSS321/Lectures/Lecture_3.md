# Biconditional
- denoted by $\iff$, true when both $p$ and $q$ are true or both are false

| $p$ | $q$ | $p \iff q$ |
| --- | --- | ---------- |
| T   | T   | T          |
| T   | F   | F          |
| F   | T   | F          |
| F   | F   | T          |

- in English
	- "if and only if"
	- "exactly when"
# Truth Assignment
- Assigning atomic prepositions truth values in a compound preposition
- Each row in a truth table is a truth assignment
# Precedence
- Like PEMDAS
	- $\neg$
	- $\land$
	- $\lor$ and $\oplus$
	- $\implies$
	- $\iff$
# Bitwise operations
- java operators that create new numbers by comparing individual bits of numbers
- ex)
```
int x = 5;
int y = 11;
x & y = 1
```

| $x$     | 0   | 1   | 0   | 1   |
| ------- | --- | --- | --- | --- |
| $y$     | 1   | 0   | 1   | 1   |
| $x$&$y$ | 0   | 0   | 0   | 1   |
# Puzzles
- q: you can ride the rollercoaster
- r: you are under 4ft tall
- s: you are older than 16
$r\land \neg s\implies \neg q$ 

# Propositional Equivalences
- A *tautology* is a compound proposition that is true under all truth assignments
- Compound propositions that have the same truth value under all truth assignments are called *logically equivalent*
	- Or, compound propositions $p$ and $q$ are logically equivalent if $p \iff q$ is a tautology
	- We denote $p$ and $q$ as $p\equiv q$
## DeMorgan's Laws
$\neg(p\land q)\equiv \neg p\lor \neg q$
$\neg(p\lor q)\equiv \neg p\land \neg q$
## Other laws
- $(p\implies q)\land(p\implies r)\equiv p\implies(q\land r)$
- $\land_{j=1}^nP_{j}=p_{1}\land p_{2}\land\dots \land p_{n}$
- 