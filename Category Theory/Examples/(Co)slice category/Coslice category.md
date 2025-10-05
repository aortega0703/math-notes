---
tags:
  - definition
  - theorem
  - math/category_theory
related topics:
  - "[[Slice category]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
For a [[Category]] $cal(C)$ and an object $A in op("ob")(cal(C))$, the _coslice category_ (or sometimes _under category_) $A/cal(C)$ is defined by the data
- Objects:
	$$op("obj")(A/cal(C)) = \{f in op("arr")(cal(C))\ |\ op("Dom")(f)=A\}$$
	morphisms in $cal(C)$ from $A$.
- Morphisms:
	$$op("Hom")_{cal(C)/A}(f : A -> B,\ g: A -> C) = \{\alpha in op("Hom")_{cal(C)}(B, C)\ |\ g = \alpha f\}$$
	morphisms $\alpha$ such that the following commutes
	![[Coslice category definition.png]]
- Composition as usual.
The [[Opposite category|Dual]] notion is an [[Slice category]].
---
This data does describe a category.
##### Proof:
Let $f,g,h,i inop("obj")(A/cal(C))$ and $f\overset{\alpha}{ -> }g\overset{\beta}{ -> }h\overset{\gamma}{ -> }i$, in $cal(C)$ as
![[Coslice category proof.png]]
- Identity:
	Consider $op("id")_B:B -> B$, $f=op("id")_B f$ by [[Identity function is unital]] so $op("id")_B: f -> f$ in $A/cal(C)$.
- Composition:
	By definition $g=\alpha f$ and $h=\beta g$. Then $h=\beta(\alpha f) = (\beta\alpha) f$ so $\beta\alpha: f -> h$ in $A/cal(C)$.
- Unitality:
	$op("id")_C \alpha = \alpha$ and $\beta op("id")_C = \beta$ by [[Identity function is unital]].
- Associativity:
	$(\gamma \beta)\alpha = \gamma(\beta\alpha)$ by [[Function composition is associative]].
Then $A/cal(C)$ is a category.