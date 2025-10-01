---
tags:
  - definition
  - set_theory
related topics:
  - "[[Function]]"
---
For [[Function|functions]] $A \overset{f}{\to} B \overset{g}{\to} C \overset{h}{\to} D$, $h\circ(g\circ f)= (h\circ g)\circ f$ (function composition is associative). i.e. the following commutes
![[Function composition associative.png]]
##### Proof:
Let $a in A$, then$$

	\big(h\circ(g\circ f)\big)(a) 
		&= h\big((g\circ f)(a)\big)\
		&= h\big(g(f(a))\big)\
		&= (h\circ g)(f(a))\
		&= ((h\circ g)\circ f)(a)

$$So $h\circ(g\circ f)= (h\circ g)\circ f$.