---
tags:
  - definition
  - theorem
  - category_theory
  - needs_details
related topics:
  - "[[Category]]"
  - "[[Matrix multiplication]]"
---
The [[Category]] of matrices over a field $\mathbb{F}$ (denoted $\mathbf{Mat}_\mathbb{F}$) is defined as
- Objects:
	$$\operatorname{Obj}(\mathbf{Mat}) = \mathbb{N}$$
	Its objects are natural numbers.
- Morphisms:
	$$A\in\operatorname{Hom}_{\mathbf{Mat}_\mathbb{F}}(n,m) \iff A\text{ is an $n\times m$ matrix over $\mathbb{F}$}$$
	Its morphisms are matrices.
- Composition:
	For matrices $A$ $(n\times m)$ and $B$ $(m\times p)$$$
		AB \in \operatorname{Hom}_{\mathbf{Mat}_\mathbb{F}}(n,p)
	$$Its composition is given by matrix multiplication.
---
$\mathbf{Mat}_\mathbb{F}$ is a category.
##### Proof:
- Identity:
	Let $n\in\operatorname{Obj}(\mathbf{Mat}_\mathbb{F})$, then $I_n\in\operatorname{Hom}_{\mathbf{Mat}_\mathbb{F}}(n,n)$ where $I_n$ is the [[Identity matrix]] of dimensions $n\times n$.
- Composition:
	Let $A,B$ be $n\times m$ and $m\times p$ matrices respectively. Then $AB$ is a $n\times p$ matrix, so $AB \in \operatorname{Hom}_{\mathbf{Mat}_\mathbb{F}}(n,p)$.
- Unitality:
	Let $n\overset{A}{\to}m\overset{B}{\to}p$, then $I_m B =B$ and $A I_m = A$.
- Associativity:
	Matrix multiplication is associative.
Therefore $\mathbf{Mat}_\mathbb{F}$ is a category.