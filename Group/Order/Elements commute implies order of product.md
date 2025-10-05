---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Group]]"
  - "[[Order]]"
---
For elements $g,h$ in a [[Group]], 
- if $gh=hg$, then $|gh|$ divides $\text{lcm}(|g|,|h|)$.
- if additionally $\gcd(|g|, |h|)=1$, then $|gh|=|g||h|$.
##### Proof:
- $gh=hg$ $ ==> $ $|gh|$ divides $\text{lcm}(|g|,|h|)$:
	$$
	
		g^{\text{lcm}(|g|,|h|)} = h^{\text{lcm}(|g|,|h|)}&=e\
		g^{\text{lcm}(|g|,|h|)} h^{\text{lcm}(|g|,|h|)} &= e\
		(gh)^{\text{lcm}(|g|,|h|)}&=e
			&\tag{1}
	
	$$
	where $(1)$ is by [[Law of exponents for commutative elements]], then by [[Order divides exponent]] $|gh|$ divides $\text{lcm}(|g|,|h|)$.
- $gh=hg$ and $\gcd(|g|,|h|)=1$ $ ==> $ $|gh|=|g||h|$:
	- $|gh|$ divides $|g||h|$:
		By the previous result $|gh|$ divides $\text{lcm}(|g|,|h|)=|g||h|/\gcd(|g||h|)=|g||h|$.
	- $|g||h|$ divides $|gh|$:
		$$
		
		e &= (gh)^{|gh||h|}\
		&= g^{|gh||h|}h^{|gh||h|} \tag{1}\
		&= g^{|gh||h|}
		
		$$
		where $(1)$ is by [[Law of exponents for commutative elements]]. By [[Order divides exponent]] $|g|$ divides $|gh||h|$. As $\gcd(|g|,|h|)=1$ by [[Euclid lemma generalization]] $|g|$ divides $|gh|$. Similarly $|h|$ divides $|gh|$. By [[ab Divides c If Relative Primes]] $|g||h|$ divides $|gh|$.
	As $|g||h|$ and $|gh|$ divide each other, they are equal.