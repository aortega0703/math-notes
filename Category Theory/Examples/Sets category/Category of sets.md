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
- $op("Obj")(\mathbf{Set})$ = The collection of all [[Set|sets]].
- $op("Hom")(A,B)=B^A$ for $A,B inop("ob")(\mathbf{Set})$.
- $ compose $ = [[Function|Function composition]].

---
This data does describe a [[Category]].
##### Proof:
- Identity:
	For every set $A$ there exists an [[Identity function]] $op("id")_A: A -> A$.
- Composition:
	For functions $A\overset{f}{ -> }B\overset{g}{ -> }C$ there is a function $g compose f: A -> C$ defined as in [[Function|Function composition]].
- Unitality:
	By [[Identity function is unital]].
- Associativity:
	By [[Function composition is associative]].
Therefore $\mathbf{Set}$ is a category.