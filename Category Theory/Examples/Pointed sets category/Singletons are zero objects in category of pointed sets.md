---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Category of pointed sets]]"
  - "[[Initial-final object|Zero object]]"
---
In $\mathbf{Set}^*$ singletons are [[Initial-final object|Zero objects]].
##### Proof:
- $(\{*\}, *)$ is initial:
	For any $(A,a)$ in $\mathbf{Set}^*$ there is a single morphism $f:(\{*\}, *)\to (A,a)$, defined as $f(*)=a$.
- $(\{*\}, *)$ is final:
	For any $(A,a)$ in $\mathbf{Set}^*$ there is a single morphism $f:(A,a)\to(\{*\}, *)$, defined as $f(a')=*$ for all $a' in A$.
Therefore $(\{*\},*)$ is a zero object in $\mathbf{Set}^*$.