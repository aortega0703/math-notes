---
tags:
  - theorem
  - definition
  - math/category_theory
related topics:
  - "[[Category]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
aliases:
  - Dual
---
For a [[Category]] $cal(C)$ its _opposite category_ $cal(C)^{op("op")}$ is obtained by reversing all arrows. Spelled out this means it has
- Objects:
	$$A in op("obj")(cal(C)^{op("op")}) <==> A in op("obj")(cal(C))$$
	It has the same objects as $cal(C)$.
- Morphisms:
	$$
	f in op("Hom")_{cal(C)^op("op")}(B, A) <==> 
	f in op("Hom")_{cal(C)}(A, B)
	$$
	It reverses arrow direction in $cal(C)$.
- Composition:
	If $ compose $ is composition in $cal(C)$ and $ compose ^op("op")$ is composition in $cal(C)^{op}$, then for $A\overset{f}{ -> }B\overset{g}{ -> }C$ in $cal(C)$.$$
		g compose f = f compose ^op("op") g
	$$
Two definitions are _dual_ if one is obtained by reversing all arrows from the other.

---
$cal(C)^op("op")$ is a category.
##### Proof:
- Identity:
	Consider $op("id")_A: A -> A$ in $cal(C)$, by definition $op("id")_A: A -> A$ in $cal(C)^op("op")$ too.
- Composition:
	Let $A\overset{f}{ -> }B\overset{g}{ -> }C$ in $cal(C)^op("op")$. Then in $cal(C)$ we have $C\overset{g}{ -> }B\overset{f}{ -> }A$ and $fg:C -> A$, so there exists some $gf:A -> C$ in $cal(C)^op("op")$.
- Unitality:
	Let $A\overset{f}{ -> }B\overset{g}{ -> }C$ in $cal(C)^op("op")$. Then in $cal(C)$ we have $C\overset{g}{ -> }B\overset{f}{ -> }A$, $fop("id")_B = f$, and $op("id")_B g=g$. So in $cal(C)^op("op")$ $op("id")_B f= f$ and $gop("id")_B =g$.
- Associative:
	Let $A\overset{f}{ -> }B\overset{g}{ -> }C\overset{h}{ -> }D$ in $cal(C)^op("op")$. Then in $cal(C)$ we have $D\overset{h}{ -> }C\overset{g}{ -> }B\overset{f}{ -> }A$ and $(fg)h=f(gh)$. So in $cal(C)^op("op")$ $(hg)f=h(gf)$.
Therefore $cal(C)^op("op")$ is a category.