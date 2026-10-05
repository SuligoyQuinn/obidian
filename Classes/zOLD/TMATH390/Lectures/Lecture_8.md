# Law of Total Probability and Baye's Theorem
## Law of Total Probability (Simple)
- let A and B be two events. Then the probability of B occurring can be computed as
$$
P(B)=P(B\cap A)+P(B\cap A^c)
$$
or
$$
P(B)=P(B|A)P(A)+P(B|A^c)P(A^c)
$$
## Law of Total Probability (General)
- Assume sets $A_{1}\dots A_{k}$ are collectively exhaustive and are all disjoint events. Then the probability of some event B occurring is
$$
P(B)=\sum P(B\cap A_{i})=\sum P(B|A_{i})P(A_{i})
$$
## Baye's Theorem (Simple)
- Let A and B be two events and that we know $P(B|A)$,$P(B|A^c)$, and $P(A)$ and we would like to know $P(A|B)$ Baye's Theorem states that
$$
P(A|B)=\frac{P(B|A)P(A)}{P(B)}
$$
or
$$
P(A|B)=\frac{P(B|A)P(A)}{P(B|A)P(A)+P(B|A^C)P(A^c)}
$$
