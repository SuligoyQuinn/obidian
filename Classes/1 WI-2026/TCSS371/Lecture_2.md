# Digital Circuits
- use voltage to represent bits
# Unsigned Binary Conversion
- Binary to Decimal
	- Start at largest column with 1. Work backwards dividing by two
- Decimal to Binary
	- Start at most significant bit if $2^{\text{bit}}>\text{number}$ then put $0$. Once you put a $1$, subtract $2^{\text{bit}}$ from number.
	- Divide number by base, remainder is bit value. Repeat. Least to most significant
		- Ex) $\frac{41}{2}=1$, $\frac{20}{2}=0$, $\frac{10}{2}=0$, $\frac{5}{2}=1$, $\frac{2}{2}=0$, $\frac{1}{2}=1$.
# Twos Compliment
- Take binary number minus sign bit, flip all bits, add one.
- Copy bits from right to left including the first one, then flip all remaining bits.
- Range on an $n$-bit number: $-2^{n-1}$ through $2^{n-1}-1$
## Converting
- If leading bit is $1$ take twos compliment to get positive number. Multiply base by total add most significant bit, add to total. Repeat.