# Satisfiability
- An expression is satisfiable if there is some truth assignment for which the expression is true
# Predicates
- A *predicate* is a property that the subject of the statement can have
	- think of them as propositional functions that map values to truth value
	- subjects of predicates can be anything
	- can have more than one variable
- Ex) Let $P(x)$ be the statement $x+5=30$
- Ex) Let $P(x)$ be the statement $x$ is older than $30$ years old
	- $P(Tom Hanks)$ is true
	- $P(GretaThunberg)$ is false
- n-place/n-ary predicate is a predicate with $n$ variables
# Quantification
- make statements such as
	- All actors have a fine arts degree
		- Let $F(x)$ be the statement "$x$ has a fine arts degree"
		- domain: actors
		- $\forall xF(x)$
	- All computer programmers have a CS degree
	- For every integer $x$, $x^2>0$
- *domain of discourse*/*universe of discourse*/*domain*
	- Set of possible values of a variable of a predicate
- Universal quantification of the predicate $P(x)$ is the statement "$P(x)$ for all values of $x$ in the domain"
