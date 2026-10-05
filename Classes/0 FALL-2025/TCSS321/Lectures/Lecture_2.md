# Disjunction
- *Disjunction* of propositions $p$ and $q$ denoted $p\lor q$ is the proposition "$p$ or $q$"
	- False if both $p$ and $q$ are false, true otherwise
- Inclusive or

| $p$ | $q$ | $p\lor q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | T         |
| F   | T   | T         |
| F   | F   | F         |
- Exclusive or

| $p$ | $q$ | $p\oplus q$ |
| --- | --- | ----------- |
| T   | T   | F           |
| T   | F   | T           |
| F   | T   | T           |
| F   | F   | F           |
# Conditional
- A *conditional* statement, denoted $p\implies q$ of propositions $p$ and $q$ is the proposition "if $p$ then $q$"
	- False when $p$ is true and $q$ is false, true otherwise

| $p$ | $q$ | $p\implies q$ |
| --- | --- | ------------- |
| T   | T   | T             |
| T   | F   | F             |
| F   | T   | T             |
| F   | F   | T             |
- $p$ is the *antecedent* or the *hypothesis*
- $q$ is the *consequent* or the *conclusion*
- In English
	- "if $p$, $q$"
	- "$p$ is sufficient for $q$ for $q$"
	- "$q$ if $p$"
	- "a necessary condition for $p$ is $q$"
	- "$q$ follows from $p$"
	- "$p$ only if $q$"
- *converse*: $q\implies p$
- *contrapositive*: $\neg q\implies \neg p$
	- Logically equivalent to $p\implies q$
- *inverse* $\neg p\implies \neg q$
	- contrapositive of the converse
# Exercise

| $p$ | $q$ | $p\land q$ | $\neg p\lor q$ | $(p\land q)\implies(\neg p\lor q)$ |
| --- | --- | ---------- | -------------- | ---------------------------------- |
| T   | T   | T          | T              | T                                  |
| T   | F   | F          | F              | T                                  |
| F   | T   | F          | T              | T                                  |
| F   | F   | F          | T              | T                                  |


| $p$ | $q$ | $r$ | $\neg r$ | $p\land \neg r$ | $q\lor p$ | $(p\land \neg r)\implies(q\lor p)$ |
| --- | --- | --- | -------- | --------------- | --------- | ---------------------------------- |
| T   | T   | T   | F        | F               | T         | T                                  |
| T   | T   | F   | T        | T               | T         | T                                  |
| T   | F   | T   | F        | F               | T         | T                                  |
| T   | F   | F   | T        | T               | T         | T                                  |
| F   | T   | T   | F        | F               | T         | T                                  |
| F   | T   | F   | T        | F               | T         | T                                  |
| F   | F   | T   | F        | F               | F         | T                                  |
| F   | F   | F   | T        | F               | F         | T                                  |
