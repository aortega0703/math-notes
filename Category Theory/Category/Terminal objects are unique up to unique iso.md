---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Initial-final object|Terminal object]]"
  - "[[Isomorphism]]"
---
In a [[Category]] $\mathcal{C}$, for objects $A,B$
- If $A$ and $B$ are [[Initial-final object|Initial objects]], then $A\cong B$ and the isomorphism $A\overset{\sim}{\to}B$ is unique.
- If $A$ and $B$ are [[Initial-final object|Final objects]], then $A\cong B$ and the isomorphism $A\overset{\sim}{\to}B$ is unique.
##### Proof:
- Initial $\implies$ Isomorphic:
	As $A$ is initial, there is exactly one morphism $f:A\to B$. As $B$ is initial, there is exactly one morphism $g:B\to A$. As $A$ is initial there is exactly one morphism $A\to A$, so $gf=\text{id}_A$. As $B$ is initial there is exactly one morphism $B\to B$, so $fg=\text{id}_B$. Therefore $A\cong B$ and the isomorphisms $f$ and $g$ are unique.
- Final $\implies$ Isomorphic:
	As $B$ is final, there is exactly one morphism $f:A\to B$. As $A$ is final, there is exactly one morphism $g:B\to A$. As $A$ is final there is exactly one morphism $A\to A$, so $gf=\text{id}_A$. As $B$ is final there is exactly one morphism $B\to B$, so $fg=\text{id}_B$. Therefore $A\cong B$ and the isomorphisms $f$ and $g$ are unique.
Therefore terminal objects are unique up to unique isomorphism.