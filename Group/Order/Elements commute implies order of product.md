---
tags:
  - theorem
  - abstract_algebra
related topics:
  - "[[Group]]"
  - "[[Order]]"
---
For elements $g,h$ in a [[Group]], if $gh=hg$ then $|gh|$ divides $\text{lcm}(|g|,|h|)$.
##### Proof:
$$
\begin{align}
	g^{\text{lcm}(|g|,|h|)} = h^{\text{lcm}(|g|,|h|)}&=e\\
	g^{\text{lcm}(|g|,|h|)} h^{\text{lcm}(|g|,|h|)} &= e\\
	(gh)^{\text{lcm}(|g|,|h|)}&=e
		&\tag{1}
\end{align}
$$where $(1)$ is by [[Law of exponents for commutative elements]], then by [[Order divides exponent]] $|gh|$ divides $\text{lcm}(|g|,|h|)$.