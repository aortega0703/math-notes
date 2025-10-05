---
tags:
  - definition
  - math/category_theory
related topics:
  - "[[Category]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
A [[Category|categories]] $cal(C)$ and $cal(C)'$, $cal(C)'$ is a _subcategory_ of $cal(C)$ if
- $op("Obj")(cal(C)') subset.eq op("Obj"){cal(C)}$.
- For all $A,B in op("Obj")(cal(C)')$, $op("Hom")_{cal(C)'}(A,B) subset.eq op("Hom")_{cal(C)}(A,B)$.
- Shares identities and composition with $cal(C)$.
A subcategory is _full_ when for all $A,B in op("Obj")(cal(C)')$, $op("Hom")_{cal(C)'}(A,B) = op("Hom")_{cal(C)}(A,B)$.