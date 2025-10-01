---
tags:
  - theorem
  - category_theory
related topics:
  - "[[Product]]"
  - "[[Monic-epic|Epic]]"
---
For objects $A,B,X$, if there are arrows $f,g:X\to A\times B$ such that$$
f\pi_1=g\pi_1, quad
f\pi_2=g\pi_2
$$then $f=g$ ($\pi_1$ and $\pi_2$ are said to be _jointly epic_).
##### Proof:
There are functions $A\overset{f\pi_1=g\pi_1}{\gets} X \overset{f\pi_2=g\pi_2}{\to}B$, then there is a unique function $h:X\to A\times B$ such that the following commutes
![[jointly epic.png]]
Note that both $f$ and $g$ make the diagram commute, so $h$ being unique implies that $f=g$.