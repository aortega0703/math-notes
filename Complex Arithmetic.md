---
tags:
  - theorem
  - math/algebra
---
For the [[Complex Numbers]] ($\mathbb{C}$):
- Addition is commutative and associative, has $0$ as an identity, and every number $\alpha = a + bi$ has as an additive inverse $-\alpha = -a -bi$.
- Multiplication is commutative and associative, has $1$ as an identity, and every number $\alpha = a + bi \neq 0$ has as a multiplicative inverse $\alpha^{-1}=\frac{a}{a^2 + b^2} + \frac{b}{a^2 + b^2}i$.
- Multiplication distributes over addition.
# Proof
- Commutativity:
	- Addition:$$
	\begin{align}
		(a + bi) + (c + di) &= (a + c) + (b + d)i\\
		&= (c + a) + (d + b)i\\
		&= (c + di) + (a + bi)
	\end{align}
$$
	- Multiplication:$$
	\begin{align}
		(a + bi)(c + di) &= (ac - bd) + (ad + bc)i\\
		&= (ca - db) + (da + cb)i\\
		&= (c + di) (a + bi)
	\end{align}
$$
- Associativity:
	- Addition:$$
	\begin{align}
		&(a_1 + b_1 i) + \big((a_2 + b_2 i) + (a_3 + b_3 i)\big)\\ 
		&= (a_1 + b_1 i) + \big((a_2 + a_3) + (b_2 + b_3)i\big)\\
		&= \Big(\big(a_1 + (a_2 + a_3)\big) + \big(b_1 + (b_2 + b_3)\big)i\Big)\\
		&= \Big(\big((a_1 + a_2) + a_3\big) + \big((b_1 + b_2) + b_3\big)i\Big)\\
		&= \big((a_1 + a_2) + (b_1 + b_2)i\big) + (a_3 + b_3 i)\\
		&= \big((a_1 + b_1 i) + (a_2 + b_2 i)\big) + (a_3 + b_3 i)
	\end{align}
$$
	- Multiplication:$$
	\begin{align}
		&(a_1 + b_1 i) \big((a_2 + b_2 i) (a_3 + b_3 i)\big)\\
		&= (a_1 + b_1 i) \big((a_2 a_3 - b_2 b_3) + (a_2 b_3 + b_2 a_3)i\big)\\
		&= \big(a_1 (a_2 a_3 - b_2 b_3) - b_1 (a_2 b_3 + b_2 a_3)\big) 
		+ \big(a_1 (a_2 b_3 + b_2 a_3)+ b_1 (a_2 a_3 - b_2 b_3)\big)i\\
		&=\big((a_1 a_2 - b_1 b_2) a_3 - (a_1 b_2 + b_1 a_2) b_3\big) 
		+ \big((a_1 a_2 - b_1 b_2) b_3 + (a_1 b_2 + b_1 a_2) a_3\big)\\
		&=\big((a_1 a_2 - b_1 b_2) + (a_1 b_2 + b_1 a_2)i\big)(a_3 + b_3 i)\\
		&=\big((a_1 + b_1 i)(a_2 + b_2 i)\big)(a_3 + b_3 i)
	\end{align}
$$
- Existence of identity:
	- Addition:$$
	\begin{align}
		(a + bi) + 0
		&= (a + 0) + (b + 0)i\\
		&= a + bi
	\end{align}
$$
	- Multiplication:$$
	\begin{align}
		(a + bi)1
		&= (a \cdot 1 - b \cdot 0) + (a \cdot 0 + b \cdot 1)i\\
		&= a + bi
	\end{align}
$$
- Existence of inverses:
	- Addition:$$
	\begin{align}
		(a + bi) + \big(- (a + bi)\big)
		&= (a + bi) + \big(- a + (-b)i\big)\\
		&= (a + (-a)) + (b + (-b))i\\
		&= 0 + 0i = 0
	\end{align}
$$
	- Multiplication:$$
	\begin{align}
		(a + bi)(a + bi)^{-1}
		&= (a + bi)\left(\frac{a}{a^2 + b^2} + \frac{-b}{a^2 + b^2}i\right)\\
		&= \left(\frac{a^2}{a^2 + b^2} + \frac{b^2}{a^2 + b^2}\right)
		+ \left(\frac{-ab}{a^2 + b^2} + \frac{ab}{a^2 + b^2}\right)i\\
		&= 1 + 0i = 1
	\end{align}
$$
- Distributivity:$$
	\begin{align}
		&(a_1 + b_1i)\big((a_2 + b_2 i) + (a_3 + b_3 i)\big)\\
		&= (a_1 + b_1i) \big((a_2 + a_3) + (b_2 + b_3)i\big)\\
		&= \big(a_1 (a_2 + a_3) - b_1 (b_2 + b_3)\big)
		+ \big(a_1 (b_2 + b_3) + b_1 (a_2 + a_3)\big)i\\
		&= \big((a_1 a_2 - b_1 b_2) + (a_1 a_3 - b_1 b_3)\big)
		+ \big((a_1 b_2 + b_1 a_2) + (a_1 b_3 + b_1 a_3)\big)i\\
		&= \big((a_1 a_2 - b_1 b_2) + (a_1 b_2 + b_1 a_2)i\big)
		+ \big((a_1 a_3 - b_1 b_3) + (a_1 b_3 + b_1 a_3)i\big)\\
		&= (a_1 + b_1i) (a_2 + b_2 i) + (a_1 + b_1 i) (a_3 + b_3 i)
	\end{align}
$$