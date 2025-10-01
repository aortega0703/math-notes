---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Order]]"
---
For a [[Group]] $G$ and $g,h in G$, $|gh|=|hg|$.
##### Proof:
- $(aga^{-1})^n=ag^na^{-1}$:
	By induction on $n$.
	- $\mathcal{P}(0)$:
		$ag^0a^{-1}=aa^{-1}=e=(aga^{-1})^0$.
	- $\mathcal{P}(n)\implies\mathcal{P}(n+1)$:
		$$
		
			(aga^{-1})^{n+1} 
			&= (aga^{-1})^naga^{-1}\
			&= ag^na^{-1}aga^{-1}
				&\text{by induction}\
			&= ag^nga^{-1}\
			&= ag^{n+1}a^{-1}
		
		$$
	So $(aga^{-1})^n=ag^na^{-1}$ for all $n$.
- $|aga^{−1} | = |g|$:
	- $|aga^{-1}| lt.eq |g|$:
		$(aga^{-1})^{|g|}=ag^{|g|}a^{-1}=aa^{-1}=e$, so $|aga^{-1}| lt.eq |g|$.
	- $|g| lt.eq|aga^{-1}|$:
		Let $|aga^{-1}|=n$, then$$
	
		e &= (aga^{-1})^n\
		&= ag^na^{-1}\
		a&=ag^n\
		e&=g^n
	
	$$So $|g| lt.eq n=|aga^{-1}|$.
	Then $|aga^{−1} | = |g|$.
- $|gh| = |hg|$:
	$|gh|=|g(hg)g^{-1}| = hg$.