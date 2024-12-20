---
tags:
  - definition
  - category_theory
related topics:
  - "[[Category|Object]]"
  - "[[Category|Morphism]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
aliases:
  - Initial object
  - Final object
  - Terminal object
  - Zero object
---
In a [[Category]] $\mathcal{C}$
- An object $I$ is _initial_ when for any object $A$ in $\mathcal{C}$ there exists exactly one morphism $I\to A$, i.e.$$
\forall A\in\operatorname{Obj}(\mathcal{C}). \big|\text{Hom}_\mathcal{C}(I,A)\big|=1
$$
- An object $F$ is _final_ when for any object $A$ in $\mathcal{C}$ there exists exactly one morphism $A\to F$, i.e.$$
\forall A\in\operatorname{Obj}(\mathcal{C}). \big|\text{Hom}_\mathcal{C}(A,F)\big|=1
$$
- An object $T$ is _terminal_ if its either initial or final.
- An object $Z$ is a _zero object_ when its both initial and final.
Initial and final objects are [[Opposite category|Dual]] concepts.