# Complete Memory Addressing Modes
## General Form
$$
D(R_{b},R_{i},S)
$$
$D$: Constant displacement
	1, 2, or 4 bytes
$R_{b}$: Base register
$R_{i}$: Index register
	Cannot be `%rsp/%esp`
$S$: Scale
	1, 2, or 4 bytes
$$
Mem[\mathrm{Re}g[R_{b}]+S\cdot \mathrm{Re}g[R_{i}]+ D]
$$
## Special Cases
$$
(R_{b},R_{i})\to Mem[\mathrm{Re}g[R_{b}]+\mathrm{Re}g[R_{i}]]
$$
$$
D(R_{b},R_{i})\to Mem[\mathrm{Re}g[R_{b}]+\mathrm{Re}g[R_{i}]+D]
$$
$$
(R_{b},R_{i},S)\to Mem[\mathrm{Re}g[R_{b}]+S\cdot \mathrm{Re}g[R_{i}]]
$$
# Arithmetic and Control
## Load Effective Address: lea
- `leal` Source, Destination
	- Source is address mode expression
	- Set Destination to address denoted by expression
- Uses
	- Computing addresses without a memory reference
	- Computing arithmetic expressions of the form $x+k\cdot y$
## Some Arithmetic Operations
- Two operand instructions
	- `addl` $Dest=Dest+Src$
	- `subl`$Dest=Dest-Src$
	- `imull`$Dest=Dest\cdot Src$
	- `sall`$Dest=Dest\ll Src$
	- `sarl`$Dest=Dest\gg Src$
		- Arithmetic Right Shift, fills with sign bit
	- `shrl`$Dest=Dest\gg Src$
		- Logical Right Shift, fills with $0$
	- `xorl`$Dest=Dest \textasciicircum Src$
	- `andl`$Dest=Dest \cap Src$
	- `orl`$Dest = Dest\cup Src$
- One operand instructions
	- `incl`$Dest = Dest+1$ 
	- `decl`$Dest=Dest-1$
	- `negl`$Dest=-Dest$
	- `notl`$Dest=\neg Dest$
## Condition Codes
- Status of recent tests
- Single bit registers
	- `ZF` last operation resulted in a zero
	- `SF` last operation resulted in a negative value
		- equals to the value of the sign bit
	- `CF` last operation resulted in an unsigned overflow
	- `OF` last operation caused a two's complement overflow
- NOT set by `LEA`
- Explicit Setting
	- `CMPL Src1 Src2`
		- Computes $Src2-Src 1$
		- Does not change either operands
	- `TESTL Src1 Src2`
		- Computes $Src 2\cap Src 1$
		- Does not change either operand
		- Often arguments are the same or one is a bit mask
### Accessing Condition Codes
`setX` instructions

| SetX  | Condition | Description          |
| ----- | --------- | -------------------- |
| sete  |           | Equal/Zero           |
| setne |           | Not Equal / Not Zero |
| sets  |           | Negative             |
| setns |           | Nonnegative          |
| setg  |           | Greater (Signed)     |
| setge |           | Greater or Equal (S) |
| setl  |           | Less (S)             |
| setle |           | Less or Equal (S)    |
| seta  |           | Above (Unsigned)     |
| setb  |           | Below (U)            |
## Loops
- Use conditional branch to either continue looping or exit loop

