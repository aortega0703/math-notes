---
tags:
  - definition
  - theorem
  - category_theory
related topics:
  - "[[Category]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
For a [[Category]] $\mathcal{C}$ and an object $A\in \operatorname{ob}(\mathcal{C})$, the _slice category_ $\mathcal{C}/A$ is defined by the data
- $\displaystyle\operatorname{obj}(\mathcal{C}/A) = \bigcup_{S\in\operatorname{obj}(\mathcal{C})} \operatorname{Hom}_\mathcal{C}(S, A)$
- $\operatorname{Hom}_{\mathcal{C}/A}(f : B \to A,\ g: C \to A) = \{\alpha \in \operatorname{Hom}_{\mathcal{C}}(B, C)\ |\ f = g\alpha\}$
- Composition as usual.
The morphisms in $\mathcal{C}/A$ are those $\alpha$ such that the following commutes
![[Slice category definition.png]]

---
This data does describe a category.
##### Proof:
Let $f,g,h,i\in\operatorname{obj}(\mathcal{C}/A)$ and $f\overset{\alpha}{\to}g\overset{\beta}{\to}h\overset{\gamma}{\to}i$, in $\mathcal{C}$ as
![[Slice category proof.png]]
- Identity:
	Consider $\operatorname{id}_B: B\to B$ in $\mathcal{C}$, $f=\operatorname{id}_B f$ by [[Identity function is unital]] so $\operatorname{id}_B:f\to f$ in $\mathcal{C}/A$.
- Composition:
	By definition $f=g\alpha$ and $g=h\beta$. Then $f=(h\beta)\alpha=h(\beta\alpha)$, so $\beta\alpha:f\to g$ in $\mathcal{C}/A$.
- Unitality:
	$\operatorname{id}_C \alpha = \alpha$ and $\beta\operatorname{id}_C=\beta$ by [[Identity function is unital]].
- Associativity:
	$(\gamma\beta)\alpha = \gamma(\beta\alpha)$ by [[Function composition is associative]].
Then $\mathcal{C}/A$ is a category.