# More matrices and relations
## Matrix Operations
- Addition
	- $A_{nxn}+B_{nxn}$
	- $\begin{bmatrix}a_{1,1}a_{1,n} \\ a_{n,1}a_{n,n}\end{bmatrix}+\begin{bmatrix}b_{1,1}b_{1,n} \\ b_{n,1}b_{n,n}\end{bmatrix}=\begin{bmatrix}a_{1,1}+b_{1,1} a_{1,n}+b_{1,n} \\ a_{n,1}+b_{n,1} a_{n,n}+b_{n,n}\end{bmatrix}$
- Multiplication
	- $A_{m\times k}\cdot B_{k\times n}=C_{m\times n}$
	- $C_{i,j}=\sum^n_{k=1}a_{i,k}\cdot b_{k,j}$
- Associative
	- $(A\cdot B)C=A(B\cdot C)$
- Not Commutative
	- $A\cdot B\neq B\cdot A$
## 0-1 Matrix
- Join
	- $A\lor B=C$
	- $C_{m,n}=A_{m,n}\lor B_{m,n}$
- Meet
	- $A\land B=C$
	- $C_{m,n}=(A_{m,1}\land B_{1,n})\lor(A_{m,2}\land B_{2,n})\lor\dots \lor(A_{m,n}\land B_{m,n})$
## Closure
- Minimal relation that contains the original relation plus whatever property
- Ex) the reflexive closure of $R$ is the minimal relation that contains $R$ and is reflexive