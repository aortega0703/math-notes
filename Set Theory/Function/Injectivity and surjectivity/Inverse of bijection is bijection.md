---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Injectivity and surjectivity|Bijectivity]]"
---
For a [[Injectivity and surjectivity|Bijection]] $f:A\overset{\sim}{\to}B$, $f^{-1}:B\overset{\sim}{\to}A$ is also a bijection.
##### Proof:
- Injective:
	By [[Bijective iff inverse]] $f\circ f^{-1}=\operatorname{id}_B$ so $f$ is a left inverse of $f^{-1}$, by [[Injective iff left inverse]] $f^{-1}$ is injective.
- Surjective:
	By [[Bijective iff inverse]] $f^{-1}\circ f=\operatorname{id}_A$ so $f$ is a right inverse of $f^{-1}$, by [[Surjective iff right inverse]] $f^{-1}$ is surjective.
So $f^{-1}$ is bijective.