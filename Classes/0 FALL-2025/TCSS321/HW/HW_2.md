Quinn Suligoy
# 1
$m\implies(e\lor p)$

"You can see the movie" **only if** "you are over 18 years old" **or** "you have the permission of a parent"

$a$ **only if** $b$ translates to $a\implies b$ therefore the logical proposition must take the form $m\implies\dots$. From there  "you are over 18 years old" **or** "you have the permission of a parent" can be transformed into $e\lor p$. Making the total logical proposition $m\implies(e\lor p)$. Where $(e\lor p)$ is evaluated first.
# 2
$p$: you prepare your taxes carefully
$q$: you will pay more taxes than you need to
$r$: you will be thrown in jail for tax evasion
$\neg p\implies(q\lor r)$
# 3
## a
$p$: it is raining in Minneapolis
$q$: it is snowing in Buffalo
$r$: it is foggy in Seattle
## b
$(p\land \neg q)\implies r$
$r\iff \neg q$
$q$
## c

| $p$   | $q$   | $r$   | $\neg q$ | $(p\land \neg q)$ | $(p\land \neg q)\implies r$ | $r\iff \neg q$ | $q$   |
| ----- | ----- | ----- | -------- | ----------------- | --------------------------- | -------------- | ----- |
| T     | T     | T     | F        | F                 | T                           | F              | T     |
| **T** | **T** | **F** | **F**    | **F**             | **T**                       | **T**          | **T** |
| T     | F     | T     | T        | T                 | T                           | T              | F     |
| T     | F     | F     | T        | T                 | F                           | F              | F     |
| F     | T     | T     | F        | F                 | T                           | F              | T     |
| **F** | **T** | **F** | **F**    | **F**             | **T**                       | **T**          | **T** |
| F     | F     | T     | T        | F                 | T                           | T              | F     |
| F     | F     | F     | T        | F                 | T                           | F              | F     |
No we cannot, assuming all statements are true $p$ can either be true or false. For all statements to be true either it is raining in Minneapolis, it is snowing in Buffalo, and it is not foggy in Seattle. Or it is not raining in Minneapolis, it is snowing in Buffalo, and it is not foggy in Seattle.
# 4
## a
$p$: Priya joins the computer science club
$q$: Quienten joins the computer club
$r$: Rosalita joins the computer club
## b
$(p\lor q)\implies r$
$q\implies \neg p$
$p \iff r$

| $p$   | $q$   | $r$   | $p\lor q$ | $(p\lor q)\implies r$ | $q\implies \neg p$ | $p \iff r$ |
| ----- | ----- | ----- | --------- | --------------------- | ------------------ | ---------- |
| T     | T     | T     | T         | T                     | F                  | T          |
| T     | T     | F     | T         | F                     | F                  | F          |
| **T** | **F** | **T** | **T**     | **T**                 | **T**              | **T**      |
| T     | F     | F     | T         | F                     | T                  | F          |
| F     | T     | T     | T         | T                     | T                  | F          |
| F     | T     | F     | T         | F                     | T                  | T          |
| F     | F     | T     | F         | T                     | F                  | F          |
| F     | F     | F     | F         | T                     | F                  | T          |

# c
Yes, if Priya and Rosalita join and Quienten does not, then all three statements are true
# 5
## a

| $p$ | $q$ | $r$ | $\neg r$ | $q\land \neg r$ | $\neg p$ | $(q\land \neg r)\lor \neg p$ |
| --- | --- | --- | -------- | --------------- | -------- | ---------------------------- |
| T   | T   | T   | F        | F               | F        | F                            |
| T   | T   | F   | T        | T               | F        | T                            |
| T   | F   | T   | F        | F               | F        | F                            |
| T   | F   | F   | T        | F               | F        | F                            |
| F   | T   | T   | F        | F               | T        | T                            |
| F   | T   | F   | T        | F               | T        | T                            |
| F   | F   | T   | F        | F               | T        | T                            |
| F   | F   | F   | T        | F               | T        | T                            |
## b
$$
\neg a\lor b\equiv a\implies b
$$
$$
(q\land \neg r)\lor \neg p\equiv p\implies(q\land \neg r)
$$

# 6
## a

| $p$ | $q$ | $p \iff q$ | $p\lor q$ | $(p \iff q)\iff(p\lor q)$ | $p\land q$ |
| --- | --- | ---------- | --------- | ------------------------- | ---------- |
| T   | T   | T          | T         | T                         | T          |
| T   | F   | F          | T         | F                         | F          |
| F   | T   | F          | T         | F                         | F          |
| F   | F   | T          | F         | F                         | F          |
## b
$$
p\land q
$$
I'm not going to do the algebra for this one

| $(p \iff q)\iff(p\lor q)$ | $p\land q$ |
| ------------------------- | ---------- |
| T                         | T          |
| F                         | F          |
| F                         | F          |
| F                         | F          |
# 7
I've taken TMATH300 which introduced concepts such as logical propositions, logical operators, logical equivalence, and universal quantification. These concepts were usually done using sets but the core logic is the same. The only new thing I think we have covered is predicates.