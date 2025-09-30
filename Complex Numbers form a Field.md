---
tags:
  - theorem
  - math/algebra
---
For the [[Complex Numbers]] ($CC$):
- Addition is commutative and associative, has $0$ as an identity, and every number $alpha = a + b i$ has as an additive inverse $-alpha = -a -b i$.
- Multiplication is commutative and associative, has $1$ as an identity, and every number $alpha = a + b i != 0$ has as a multiplicative inverse $alpha^(-1) = a / (a^2 + b^2) + b / (a^2 + b^2)i$.
- Multiplication distributes over addition.
# Proof
- Commutativity:
	- Addition:$$
		(a + b i) + (c + d i) &= (a + c) + (b + d)i\
		&= (c + a) + (d + b)i\
		&= (c + d i) + (a + b i)
$$
	- Multiplication:$$
		(a + b i)(c + d i) &= (a c - b d) + (a d + b c)i\
		&= (c a - d b) + (d a + c b)i\
		&= (c + d i) (a + b i)
$$
- Associativity:
	- Addition:$$
		&(a_1 + b_1 i) + ((a_2 + b_2 i) + (a_3 + b_3 i))\
		&= (a_1 + b_1 i) + lr(((a_2 + a_3) + (b_2 + b_3)i), size: #150%)\
		&= lr((a_1 + (a_2 + a_3)), size: #150%) 
		+ lr((b_1 + (b_2 + b_3)), size: #150%)i\
		&= lr(((a_1 + a_2) + a_3), size: #150%)
		+ lr(((b_1 + b_2) + b_3), size: #150%)i\
		&=lr(((a_1 + a_2) + (b_1 + b_2)i), size: #150%)
		+ (a_3 + b_3 i)\
		&= lr(((a_1 + b_1 i) + (a_2 + b_2 i)), size: #150%)
		+ (a_3 + b_3 i)
$$
	- Multiplication:$$
		&(a_1 + b_1 i) lr(((a_2 + b_2 i) (a_3 + b_3 i)), size: #150%)\
		&= (a_1 + b_1 i)
		lr(((a_2 a_3 - b_2 b_3) + (a_2 b_3 + b_2 a_3)i), size: #150%)\
		&= lr((a_1 (a_2 a_3 - b_2 b_3) - b_1 (a_2 b_3 + b_2 a_3)), size: #150%)
		+ lr((a_1 (a_2 b_3 + b_2 a_3)+ b_1 (a_2 a_3 - b_2 b_3)), size: #150%)i\
		&= lr(((a_1 a_2 - b_1 b_2) a_3 - (a_1 b_2 + b_1 a_2) b_3), size: #150%)
		+ lr(((a_1 a_2 - b_1 b_2) b_3 + (a_1 b_2 + b_1 a_2) a_3), size: #150%)i\
		&= lr(((a_1 a_2 - b_1 b_2) + (a_1 b_2 + b_1 a_2)i), size: #150%)
		(a_3 + b_3 i)\
		&= lr(((a_1 + b_1 i)(a_2 + b_2 i)), size: #150%)
		(a_3 + b_3 i)
$$
- Existence of identity:
	- Addition:$$
		(a + b i) + 0
		&= (a + 0) + (b + 0)i\
		&= a + b i
$$
	- Multiplication:$$
		(a + b i)1
		&= (a dot 1 - b \cdot 0) + (a dot 0 + b dot 1)i\
		&= a + b i
$$
- Existence of inverses:
	- Addition:$$
		(a + b i) - (a + b i)
		&= (a + b i) + (- a - b i)\
		&= (a - a) + (b - b)i\
		&= 0 + 0 i = 0
$$
	- Multiplication:$$
		(a + b i)(a + b i)^(-1)
		&= (a + b i)(a / (a^2 + b^2) + -b / (a^2 + b^2) i)\
		&= ((a^2) / (a^2 + b^2) + (b^2) / (a^2 + b^2))
		+ ((-a b) / (a^2 + b^2) + (a b) / (a^2 + b^2))i\
		&= 1 + 0i = 1
$$
- Distributivity:$$
		&(a_1 + b_1i) lr(((a_2 + b_2 i) + (a_3 + b_3 i)), size: #150%)\
		&= (a_1 + b_1i) lr(((a_2 + a_3) + (b_2 + b_3)i), size: #150%)\
		&= lr((a_1 (a_2 + a_3) - b_1 (b_2 + b_3)), size: #150%)
		+ lr((a_1 (b_2 + b_3) + b_1 (a_2 + a_3)), size: #150%)i\
		&= lr(((a_1 a_2 - b_1 b_2) + (a_1 a_3 - b_1 b_3)), size: #150%)
		+ lr(((a_1 b_2 + b_1 a_2) + (a_1 b_3 + b_1 a_3)), size: #150%)i\
		&= lr(((a_1 a_2 - b_1 b_2) + (a_1 b_2 + b_1 a_2)i), size: #150%)
		+ lr(((a_1 a_3 - b_1 b_3) + (a_1 b_3 + b_1 a_3)i), size: #150%)\
		&= (a_1 + b_1i) (a_2 + b_2 i) + (a_1 + b_1 i) (a_3 + b_3 i)
$$