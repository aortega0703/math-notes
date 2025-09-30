---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Cyclic group]]"
  - "[[Order]]"
mathLink: $b\in\langle a \rangle \implies |b|$ divides $|a|$
---
In a finite [[Cyclic group]] $G$, the order of an element $a\in G$ divides the order of the group.
##### Proof:
$a=g^n$ where $g$ is the generator of $G$ and $n\in\mathbb{Z}$, by [[Order of power element]] $|a| = |g|/\operatorname{gcd}(|g|,n)$ so $|a|$ divides $|g|$ and by [[Order of cyclic group is order of generator]] $|a|$ divides $|G|$.