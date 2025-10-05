---
tags:
  - theorem
  - math/set_theory
related topics:
  - "[[Identity function]]"
---
For $A\overset{f}{ -> } B\overset{g}{ -> }C$$$
g compose op("id")_B=g, quad op("id")_B compose f = f$$
which is to say, the following commute
![[Identity function left cancel.png]]![[Identity function right cancel.png]]
##### Proof:
- $g compose op("id")_B=g$:
	Let $b in B$, then$$
	
		(g compose op("id")_B)(b) 
			&= g(op("id")_B(b))\
			&= g(b)\
		g compose op("id")_B &= g
	
	$$
- $op("id")_B compose f = f$:
	Let $a in A$, then$$
	
		(op("id")_B compose f)(a)
			&= op("id")_B(f(a))\
			&= f(a)\
		op("id")_B compose f &= f
	
	$$