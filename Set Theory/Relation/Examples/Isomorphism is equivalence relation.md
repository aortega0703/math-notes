---
tags:
  - theorem
  - category_theory
related topics:
  - "[[Isomorphism]]"
  - "[[Equivalence relation]]"
---
For a [[Category]] $\mathcal{C}$, [[Isomorphism]] ($\cong$) defines an [[Equivalence relation]] in $\operatorname{Obj}(\mathcal{C})$.
##### Proof:
- Reflexivity:
	By [[Identity is iso]] $\operatorname{id}_A: A\overset{\sim}{\to}A$ is an isomorphism, so $A\cong A$.
- Commutativity:
	Let $A\cong B$, then there exists some isomorphism $f:A\overset{\sim}{\to} B$. By [[Inverse is iso]] $f^{-1}:B\overset{\sim}{\to}A$ is also an isomorphism so $B\cong A$.
- Transitivity:
	Let $A\cong B$ and $B\cong C$, then there exist isomorphisms $A\overset{f}{\to} B\overset{g}{\to}C$. By [[Composition of isos is iso]] $gf:A\overset{\sim}{\to}C$ is an isomorphism so $A\cong C$.
Then $\cong$ is an equivalence relation in $\operatorname{Obj}(\mathcal{C})$.