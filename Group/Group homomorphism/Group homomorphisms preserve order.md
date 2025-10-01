---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Group homomorphism]]"
  - "[[Order]]"
---
Let $\phi: G\to H$ be a [[Group homomorphism]] and let $g in G$ an element of finite [[Order]]. Then$$
	|\phi(g)| \text{ divides } |g|
$$
##### Proof:
For any $n>0 in ZZ$, as $\phi$ is an homomorphism then $\phi(g)^n=\underbrace{\phi(g)\dots\phi(g)}_{n \text{ times}}=\phi(g^n)$, so $\phi(g)^{|g|}=\phi(g^{|g|})=\phi(e_G)=e_H$. By [[Order divides exponent]] $|\phi(g)|$ divides $|g|$.