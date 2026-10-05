# Axioms of Probability
## Unions of Events
- Union of two events A and B consists of all outcomes S that are in either A or B
$$
A\cup B
$$
## Intersections of Events
- Intersection of two events A and B consists of all outcomes in S that are in both A and B
$$
A\cap B
$$
## Compliments of Events
- The compliment of the event E is all outcomes S that are not in E
## Disjoint Events
- Events A and B are sed to be disjoint events if they do not share any elements
## De Morgan's Laws
$$
(A\cap B)^c=A^c\cup B^C
$$
$$
(A\cup B)^c=A^c\cap B^C
$$
## Axioms
1. $0 \leq P(E)\leq 1$
2. $P(S)=1$
3. If E1 and E2 are disjoint then $P(E_{1}\cup E_{2}) = P(E_{1}) + P(E_{2})$
## General Addition Rule
- for any probabilities A and B, the probability that A or B occurs is
$$
P(A\cup B)=P(A)+P(B)-P(A\cap B)
$$
### Card Example
- probability of drawing red card or king in deck of 52 cards
$$
P(A)=0.5
$$
$$
P(B)=\frac{4}{52}
$$
$$
P(A\cap B)=\frac{2}{52}

$$
$$
P(A\cup B)=\frac{1}{2}+\frac{4}{52}-\frac{2}{52}=0.5385
$$
- probability of being delt straight or flush
$$
P(A)=\frac{36*4^4}{_{52}C_{5}}
$$
$$
P(B)=\frac{_{4}C_{1}*_{13}C_{5}}{_{52}C_{5}}
$$
$$
P(A\cap B)=\frac{_{4}C_{1}*9}{_{52}C_{5}}
$$
## General Rule of Addition for 3 Sets
$$
P(A\cup B\cup C)=P(A)+P(B)+P(C)-P(A\cap B)-P(A\cap C)-P(B\cap C)+P(A\cap B\cap C)
$$
### Dice Example
A) Sum is 7
B) First die is Odd
C) Second die is Even
$$
P(A)=\frac{6}{36}
$$
$$
P(B)=\frac{3*6}{36}
$$
$$
P(C)=\frac{3*6}{36}
$$
$$
P(A\cap B)=\frac{3}{36}
$$
$$
P(A\cap C)=\frac{3}{36}
$$
$$
P(B\cap C)=\frac{9}{36}
$$
$$
P(A\cup B\cup C)=\frac{3}{36}
$$
## Complements
- sometimes easier to find the complement of an event
- The probability of event $P(E)$ is equal to $1-P(E^c)$ where $P(E^c)$ is the probability of the complement of the event E