# 1
## a
$16$
A logical operator for two variables has 4 outputs each with 2 options, True or False, therefore there are $2^4=16$ different possible logic operators for two variables.
## b and c

| $p$ | $q$ | 1   | 2   | 3   | 4   | 5   | 6   | $p\oplus q$ | 8   |
| --- | --- | --- | --- | --- | --- | --- | --- | ----------- | --- |
| T   | T   | F   | F   | F   | F   | F   | F   | F           | F   |
| T   | F   | F   | F   | F   | F   | T   | T   | T           | T   |
| F   | T   | F   | F   | T   | T   | F   | F   | T           | T   |
| F   | F   | F   | T   | F   | T   | F   | T   | F           | T   |

| $p\land q$ | $p\iff q$ | 11  | $p\implies q$ | 13  | $q\implies p$ | $p\lor q$ | 16  |
| ---------- | --------- | --- | ------------- | --- | ------------- | --------- | --- |
| T          | T         | T   | T             | T   | T             | T         | T   |
| F          | F         | F   | F             | T   | T             | T         | T   |
| F          | F         | T   | T             | F   | F             | T         | T   |
| F          | T         | F   | T             | F   | T             | F         | T   |
## d
$2^{2n}$
A logical operator with $n$ variables as an input has $2^n$ outputs each with $2$ options, True or False, therefore there are $(2^n)^2$ or $2^{2n}$ possible logic operators for two variables.
