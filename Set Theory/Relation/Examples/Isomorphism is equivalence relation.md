---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Isomorphism]]"
  - "[[Equivalence relation]]"
---
For a [[Category]] $cal(C)$, [[Isomorphism]] ($\cong$) defines an [[Equivalence relation]] in $op("Obj")(cal(C))$.
##### Proof:
- Reflexivity:
	By [[Identity is iso]] $op("id")_A: A arrow.r.tilde A$ is an isomorphism, so $A\cong A$.
- Commutativity:
	Let $A\cong B$, then there exists some isomorphism $f:A arrow.r.tilde B$. By [[Inverse is iso]] $f^{-1}:B arrow.r.tilde A$ is also an isomorphism so $B\cong A$.
- Transitivity:
	Let $A\cong B$ and $B\cong C$, then there exist isomorphisms $A\overset{f}{ -> } B\overset{g}{ -> }C$. By [[Composition of isos is iso]] $gf:A arrow.r.tilde C$ is an isomorphism so $A\cong C$.
Then $\cong$ is an equivalence relation in $op("Obj")(cal(C))$.