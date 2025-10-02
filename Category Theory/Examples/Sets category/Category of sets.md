---
tags:
  - math/category_theory
  - definition
  - theorem
related topics:
  - "[[Set]]"
  - "[[Function]]"
  - "[[Category]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
The category of sets (denoted $\mathbf{Set}$) is defined by the data
- $\operatorname{Obj}(\mathbf{Set})$ = The collection of all [[Set|sets]].
- $\operatorname{Hom}(A,B)=B^A$ for $A,B in\operatorname{ob}(\mathbf{Set})$.
- $\circ$ = [[Function|Function composition]].

---
This data does describe a [[Category]].
##### Proof:
- Identity:
	For every set $A$ there exists an [[Identity function]] $\operatorname{id}_A: A\to A$.
- Composition:
	For functions $A\overset{f}{\to}B\overset{g}{\to}C$ there is a function $g\circ f: A\to C$ defined as in [[Function|Function composition]].
- Unitality:
	By [[Identity function is unital]].
- Associativity:
	By [[Function composition is associative]].
Therefore $\mathbf{Set}$ is a category.