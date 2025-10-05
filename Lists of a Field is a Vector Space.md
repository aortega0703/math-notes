---
tags:
  - theorem
  - math/linear_algebra
---
For any [[Field]] $F$, $F^n$ (the [[Set]] of [[List]] of length $n$ of elements of $F$) form a [[Vector Space]] over $F$ with the operations:
- Addition:$$
(x_1, dots, x_n) + (y_1, dots, y_n) = (x_1 + y_1, dots, x_n + y_n)
$$
- Scalar Multiplication:$$
lambda(x_1, dots, x_n) = (lambda x_1, dots, lambda x_n)
$$
# Proof
- Commutativity:$$
(x_1, dots, x_n) + (y_1, dots, y_n) &= (x_1 + y_1, dots, x_n + y_n)\
&= (y_1 + x_1, dots, y_n + x_n)\
&= (y_1, dots, y_n) + (x_1, dots, x_n)
$$
- Associativity:
	- Vector addition:$$
	((x_1, dots, x_n) + (y_1, dots, y_n)) + (z_1, dots, z_n)
	&= (x_1 + y_1, dots, x_n + y_n) + (z_1, dots, z_n)\
	&= ((x_1 + y_1) + z_1, dots, (x_n + y_n) + z_n)\
	&= (x_1 + (y_1 + z_1), dots, x_n + (y_n + z_n))\
	&= (x_1, dots, x_n) + (y_1 + z_1, dots, y_n + z_n)\
	&= (x_1, dots, x_n) + ((y_1, dots, y_n) + (z_1, dots, z_n))
	$$
	- Scalar multiplication:$$
	(alpha beta) (x_1, dots, x_n)
	&= ((alpha beta)x_1, dots, (alpha beta)x_n)\
	&= (alpha (beta x_1), dots, alpha (beta x_n))\
	&= alpha (beta x_1, dots, beta x_n)\
	&= alpha (beta (x_1, dots, x_n))
	$$
- Distributivity:
	- Scalar multiplication over Vector addition:$$
	alpha ((x_1, dots, x_n) + (y_1, dots, y_n)) 
	&= alpha(x_1 + y_1, dots, x_n + y_n)\
	&= (alpha (x_1 + y_1), dots, alpha (x_n + y_n))\
	&= (alpha x_1 + alpha y_1, dots, alpha x_n + alpha y_n)\
	&= (alpha x_1, dots, alpha x_n) + (alpha y_1, dots, alpha y_n)\
	&= alpha (x_1, dots, x_n) + alpha (y_1, dots, y_n)
	$$
	- Scalar addition over Scalar multiplication:$$
	(alpha + beta)(x_1, dots, x_n)
	&= ((alpha + beta) x_1, dots, (alpha + beta) x_n)\
	&= (alpha x_1 + beta x_1, dots, alpha x_n + beta x_n)\
	&= (alpha x_1, dots, alpha x_n) + (beta x_1, dots, beta x_n)\
	&= alpha (x_1, dots, x_n) + beta (x_1, dots, x_n)
	$$
- Existence of identities:
	- Vector addition:$$
	(x_1, dots, x_n) + (0, dots, 0)
	&= (x_1 + 0, dots, x_n + 0)\
	&= (x_1, dots, x_n)
	$$
	- Scalar multiplication:$$
	1 (x_1, dots, x_n)
	&= (1 x_1, dots, 1 x_n)\
	&= (x_1, dots, x_n)
	$$
- Existence of inverses:$$
(x_1, dots, x_n) - (x_1, dots, x_n)
&= (x_1, dots, x_n) + (-x_1, dots, -x_n)\
&= (x_1 - x_1, dots, x_n - x_n)\
&= (0, dots, 0)
$$