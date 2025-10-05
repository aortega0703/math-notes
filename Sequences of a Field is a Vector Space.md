---
tags:
  - theorem
  - math/linear_algebra
---
For any [[Field]] $F$, $F^oo$ (the [[Set]] of [[Sequence]]s of elements of $F$) form a [[Vector Space]] over $F$ with the operations:
- Addition:$$
(x_1, x_2, dots) + (y_1, y_2, dots) = (x_1 + y_1, x_2 + y_2, dots)
$$
- Scalar Multiplication:$$
lambda(x_1, x_2, dots) = (lambda x_1, lambda x_2, dots)
$$
# Proof
- Commutativity:$$
(x_1, x_2, dots) + (y_1, y_2, dots) &= (x_1 + y_1, x_2 + y_2, dots)\
&= (y_1 + x_1, y_2 + x_2, dots)\
&= (y_1, y_2, dots) + (x_1, x_2, dots)
$$
- Associativity:
	- Vector addition:$$
	((x_1, x_2, dots) + (y_1, y_2, dots)) + (z_1, z_2, dots)
	&= (x_1 + y_1, x_2 + y_2, dots) + (z_1, z_2, dots)\
	&= ((x_1 + y_1) + z_1, (x_2 + y_2) + z_2, dots)\
	&= (x_1 + (y_1 + z_1), x_2 + (y_2 + z_2), dots)\
	&= (x_1, x_2, dots) + (y_1 + z_1, y_2 + z_2, dots)\
	&= (x_1, x_2, dots) + ((y_1, y_2, dots) + (z_1, z_2, dots))
	$$
	- Scalar multiplication:$$
	(alpha beta) (x_1, x_2, dots)
	&= ((alpha beta)x_1, (alpha beta)x_2, dots)\
	&= (alpha (beta x_1), alpha (beta x_2), dots)\
	&= alpha (beta x_1, beta x_2, dots)\
	&= alpha (beta (x_1, x_2, dots))
	$$
- Distributivity:
	- Scalar multiplication over Vector addition:$$
	alpha ((x_1, x_2, dots) + (y_1, y_2, dots)) 
	&= alpha(x_1 + y_1, x_2 + y_2, dots)\
	&= (alpha (x_1 + y_1), alpha (x_2 + y_2), dots)\
	&= (alpha x_1 + alpha y_1, alpha x_2 + alpha y_2, dots)\
	&= (alpha x_1, alpha x_2, dots) + (alpha y_1, alpha y_2, dots)\
	&= alpha (x_1, x_2, dots) + alpha (y_1, y_2, dots)
	$$
	- Scalar addition over Scalar multiplication:$$
	(alpha + beta)(x_1, x_2, dots)
	&= ((alpha + beta) x_1, (alpha + beta) x_2, dots)\
	&= (alpha x_1 + beta x_1, alpha x_2 + beta x_2, dots)\
	&= (alpha x_1, alpha x_2, dots) + (beta x_1, beta x_2, dots)\
	&= alpha (x_1, x_2, dots) + beta (x_1, x_2, dots)
	$$
- Existence of identities:
	- Vector addition:$$
	(x_1, x_2, dots) + (0, 0, dots)
	&= (x_1 + 0, x_2 + 0, dots)\
	&= (x_1, x_2, dots)
	$$
	- Scalar multiplication:$$
	1 (x_1, x_2, dots)
	&= (1 x_1, 1 x_2, dots)\
	&= (x_1, x_2, dots)
	$$
- Existence of inverses:$$
(x_1, x_2, dots) - (x_1, x_2, dots)
&= (x_1, x_2, dots) + (-x_1, -x_2, dots)\
&= (x_1 - x_1, x_2 - x_2, dots)\
&= (0, 0, dots)
$$