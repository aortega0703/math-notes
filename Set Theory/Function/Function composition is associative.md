---
tags:
  - definition
  - math/set_theory
related topics:
  - "[[Function]]"
---
For [[Function|functions]] $A \overset{f}{ -> } B \overset{g}{ -> } C \overset{h}{ -> } D$, $h compose (g compose f)= (h compose g) compose f$ (function composition is associative). i.e. the following commutes
![[Function composition associative.png]]
##### Proof:
Let $a in A$, then$$

	\big(h compose (g compose f)\big)(a) 
		&= h\big((g compose f)(a)\big)\
		&= h\big(g(f(a))\big)\
		&= (h compose g)(f(a))\
		&= ((h compose g) compose f)(a)

$$So $h compose (g compose f)= (h compose g) compose f$.