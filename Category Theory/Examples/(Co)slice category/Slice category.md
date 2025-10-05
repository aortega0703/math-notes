---
tags:
  - definition
  - theorem
  - math/category_theory
related topics:
  - "[[Category]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
For a [[Category]] $cal(C)$ and an object $A in op("ob")(cal(C))$, the _slice category_ (or sometimes _over category_) $cal(C)/A$ is defined by the data
- Objects:
	$$\displaystyleop("obj")(cal(C)/A) = \bigcup_{S inop("obj")(cal(C))} op("Hom")_cal(C)(S, A)$$
	morphisms in $cal(C)$ into $A$ 
- Morphisms:
	$$op("Hom")_{cal(C)/A}(f : B -> A,\ g: C -> A) = \{\alpha in op("Hom")_{cal(C)}(B, C)\ |\ f = g\alpha\}$$
	morphisms $\alpha$ in $cal(C)$ such that the following commutes
	![[Slice category definition.png]]
- Composition as usual.
The [[Opposite category|Dual]] notion is [[Coslice category]].
---
This data does describe a category.
##### Proof:
Let $f,g,h,i inop("obj")(cal(C)/A)$ and $f\overset{\alpha}{ -> }g\overset{\beta}{ -> }h\overset{\gamma}{ -> }i$, in $cal(C)$ as
![[Slice category proof.png]]
- Identity:
	Consider $op("id")_B: B -> B$ in $cal(C)$, $f=fop("id")_B$ by [[Identity function is unital]] so $op("id")_B:f -> f$ in $cal(C)/A$.
- Composition:
	By definition $f=g\alpha$ and $g=h\beta$. Then $f=(h\beta)\alpha=h(\beta\alpha)$, so $\beta\alpha:f -> g$ in $cal(C)/A$.
- Unitality:
	$op("id")_C \alpha = \alpha$ and $\betaop("id")_C=\beta$ by [[Identity function is unital]].
- Associativity:
	$(\gamma\beta)\alpha = \gamma(\beta\alpha)$ by [[Function composition is associative]].
Then $cal(C)/A$ is a category.