---
tags:
  - theorem
  - category_theory
related topics:
  - "[[Set]]"
  - "[[Function]]"
  - "[[Category]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
The category of sets (denoted $\mathbf{Set}$) is defined by the data
- $\operatorname{ob}(\mathbf{Set})$ = The collection of all [[Set|sets]].
- $\operatorname{Hom}(A,B)=B^A$ for $A,B\in\operatorname{ob}(\mathbf{Set})$.
- $\circ$ = [[Function|Function composition]].
This data indeed describes a [[Category]].
##### Proof:
- $\operatorname{ob}(\mathbf{Set})$ and $\operatorname{arr}(\mathbf{Set})$:
	The collections of all sets and all functions respectively.
- Domain and Codomain:
	For a function $f: A\to B$, its domain is $A$ and its codomain $B$.
- Identity:
	For every set $A$ there exists an [[Identity function]] $\operatorname{id}_A: A\to A$.
- Composition:
	For functions $A\overset{f}{\to}B\overset{g}{\to}C$ there is a function $g\circ f: A\to C$ defined as in [[Function|Function composition]].
- Unitality:
	By [[Identity function is unital]].
- Associativity:
	By [[Function composition is associative]].
Therefore $\mathbf{Set}$ is a category.