---
tags:
  - definition
  - math/category_theory
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
In a [[Category]] $cal(C)$
- An object $I$ is _initial_ when for any object $A$ in $cal(C)$ there exists exactly one morphism $I -> A$, i.e.$$
 forall A inop("Obj")(cal(C)). \big|\text{Hom}_cal(C)(I,A)\big|=1
$$
- An object $F$ is _final_ when for any object $A$ in $cal(C)$ there exists exactly one morphism $A -> F$, i.e.$$
 forall A inop("Obj")(cal(C)). \big|\text{Hom}_cal(C)(A,F)\big|=1
$$
- An object $T$ is _terminal_ if its either initial or final.
- An object $Z$ is a _zero object_ when its both initial and final.
Initial and final objects are [[Opposite category|Dual]] concepts.