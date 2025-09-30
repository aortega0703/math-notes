---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Order]]"
---
For a [[Group]] $G$ and any $g\in G$, $|g^{-1}|=|g|$.
##### Proof:
$|g|$ is the least positive integer $n$ such that $g^n=e$. 
- $|g^{-1}|\geq |g|$:
	$g^n\neq e$ for $n<|g|$, meaning $(g^{-1})^n=(g^n)^{-1}\neq e$, so $|g^{-1}|\geq |g|$.
- $|g^{-1}|\leq |g|$:
	$(g^{-1})^|g|=(g^|g|)^{-1}=e$, so $|g^{-1}|\leq |g|$.
Therefore $|g^{-1}|= |g|$.