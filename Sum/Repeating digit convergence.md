---
tags:
  - theorem
mathLink: $0.\overline{9}=1$
---
In base $d$, $0.\underbrace{0\dots0}_{k-1}\overline{(d-1)}_d= 0.\underbrace{0\dots01}_{k-1}{}_d$. That is 
$$
	(d-1)\sum_{i=k}^{ infty} d^{-i} = d^{-k+1}
$$
(e.g. $0.\overline{9}=1$ in base $10$).
##### Proof:
$$

	N &= (d-1) \sum_{i=k}^{ infty} d^{-i}\
	d N &= (d-1) \sum_{i=k}^{ infty} d^{-i+1}\
	&= (d-1) \sum_{j=k-1}^{ infty} d^{-j}
		&\text{taking $-j=-i+1$}\
	&= (d-1)\cdot d^{-k+1} 
		+ (d-1) \sum_{j=k}^{ infty} d^{-j}\
	&= (d-1)\cdot d^{-k+1} + N\
	(d-1)N &= (d-1)\cdot d^{-k+1}\
	N &= d^{-k+1}

$$