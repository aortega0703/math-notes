---
tags:
  - definition
  - theorem
  - category_theory
related topics:
  - "[[Slice category]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
For a [[Category]] $\mathcal{C}$ and an object $A\in \operatorname{ob}(\mathcal{C})$, the _coslice category_ (or sometimes _under category_) $A/\mathcal{C}$ is defined by the data
- Objects:
	$$\operatorname{obj}(A/\mathcal{C}) = \{f\in \operatorname{arr}(\mathcal{C})\ |\ \operatorname{Dom}(f)=A\}$$
	morphisms in $\mathcal{C}$ from $A$.
- Morphisms:
	$$\operatorname{Hom}_{\mathcal{C}/A}(f : A \to B,\ g: A \to C) = \{\alpha \in \operatorname{Hom}_{\mathcal{C}}(B, C)\ |\ g = \alpha f\}$$
	morphisms $\alpha$ such that the following commutes
	![[Coslice category definition.png]]
- Composition as usual.
The [[Dual]] notion is an [[Slice category]].
---
This data does describe a category.
##### Proof:
Let $f,g,h,i\in\operatorname{obj}(A/\mathcal{C})$ and $f\overset{\alpha}{\to}g\overset{\beta}{\to}h\overset{\gamma}{\to}i$, in $\mathcal{C}$ as
![[Coslice category proof.png]]
- Identity:
	Consider $\operatorname{id}_B:B\to B$, $f=\operatorname{id}_B f$ by [[Identity function is unital]] so $\operatorname{id}_B: f \to f$ in $A/\mathcal{C}$.
- Composition:
	By definition $g=\alpha f$ and $h=\beta g$. Then $h=\beta(\alpha f) = (\beta\alpha) f$ so $\beta\alpha: f\to h$ in $A/\mathcal{C}$.
- Unitality:
	$\operatorname{id}_C \alpha = \alpha$ and $\beta \operatorname{id}_C = \beta$ by [[Identity function is unital]].
- Associativity:
	$(\gamma \beta)\alpha = \gamma(\beta\alpha)$ by [[Function composition is associative]].
Then $A/\mathcal{C}$ is a category.