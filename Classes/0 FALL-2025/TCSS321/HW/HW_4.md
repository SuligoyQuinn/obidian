# 1
Let $n$ be an odd integer and $m$ be an even integer. By the definition of an odd integer $n=2k+1$ for some integer $k$, and by the definition of an even integer $m=2l$ for some integer $l$. Using these definitions our equation turns into $11(2k+1)^2+2k+1+(2k+1)(2l)^2+4$. Which simplifies to $11(4k^2+4k+1) + 2k + 1+ (2k+1)(4l^2)+4$ or $44k^2+46k+16+8l^2k+4l^2$. We can simplify this expression into the form $2(22k^2+23k+8+4l^2k+2l^2)$. Because integers are closed under multiplication and addition, $22k^2+23k+ 8 +4l^2k+2l^2$ is an integer, meaning the whole expression takes the form $2k$ for some integer $k$ making it even. 
# 2
We will use proof by contraposition. Let $n$ and $m$ be odd integers, that is $n=2k+1$ and $m=2l+1$ for some integers $n,l$. Using these definitions in our expression we get $3(2k+1)(2l+1) + 2k+1 + 2l+1$, which simplifies to $3(4kl+2k+2l+1) +2k+2l+2$ or $12kl+8k+8l+5$. Now we can expand $5$ into $4+1$ to get the expression $12kl+8k+8l+4+1$. Pulling a $2$ out from the elements besides $1$ we get the expression $2(6kl+4k+4l+2)+1$. As integers are closed under multiplication and addition, $6kl+4k+4l+2$ is an integer, making our expression follow the form $2k+1$ for some integer $k$ meaning the expression is even.
# 3
$P(S)=\{\emptyset,\{ 1 \},\{ 2 \},\{ 3 \},\{ 4 \},\{ 1,2 \},\{ 1,3 \},\{ 1,4 \},\{ 2,3 \},\{ 2,4 \},\{ 3,4 \},\{ 1,2,3 \},\{ 1,2,4 \},\{ 1,3,4 \}, \{ 2,3,4 \}, \{ 1,2,3,4 \} \}$
## a
False, for $S$ to be a subset of $P(S)$, $S$ would have to contain only a subset of itself, which is only possible if $S=\emptyset$, which is false.
## b
False, $S$ contains $4$ elements and $P(S)$ contains $16$, so there is no way for $P(S)\subseteq S$
## c
True, a powerset contains all subsets of a set, and a set is a subset of itself so it must be contained in the powerset.
## d
True. $S-\{ 1,2 \}$ = $\{ 3,4 \}$ which is a subset of $S$, meaning it is contained in the powerset.
## e
False. $x$ would be an element of $S$ not a subset of $S$ meaning it would not be contained in $P(S)$
# 4
$\bar{A}=\{ 4,5,6,7,8 \}$
## a
$\bar{A}\cap C=\{ 4,5 \}$ , which does not contain $4,5,6$, therefor $B$ is not a subset.
## b
$\bar{A}\cup C=\{ 3,4,5,6,7,8 \}$, which contains $4,5,6$, therefor $B$ is a subset
# 5
For this course I have not been using the textbook. In other math classes I have found it helpful to use the textbook to learn about topics before being presented in class.
# Bonus
Let $a\in \overline{X\cup Y}\cup Y$. Then $a\not \in X\cup Y$, or $a\in Y$. We can break this into the statement $\neg(a\in X\lor a\in Y)\lor a\in Y$. Then using DeMorgan's laws we can get the statement $(a\in \bar{X}\land a\in \bar{Y})\lor a\in Y$. Using the distributive property this becomes $(a\in \bar{X}\lor a\in Y)\land(a\in \bar{Y}\lor a\in Y)$. The second half of this statement is a tautology and can therefore be ignored, leaving us with the statement $a\in \bar{X}\lor a\in Y$, which can be transformed into $a\in \bar{X}\cup Y$. 
Let $a\in \bar{X}\cup Y$, then $a\not \in X$ or $a\in Y$. Meaning $a\not \in X$ or $a \not \in Y$, unless $a\in Y$. Which translates to $a\not \in X\cup Y$ or $a\in Y$. Or $a\in\overline{X\cup Y}\cup Y$.