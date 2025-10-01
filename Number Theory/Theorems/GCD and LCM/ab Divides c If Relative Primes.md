---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Divisibility]]"
  - "[[Greatest Common Divisor|Relative Prime]]"
---
For $a,b,c in ZZ$, if $a$ and $b$ divide $c$, and $a,b$ are relatively prime, then $ab$ divides $c$.
##### Proof:
By definition let $c=k_a a= k_b b$ and by [[Division algorithm]] $c = q(ab) + r$ for some $q,(0 lt.eq r < ab) in ZZ$, then:$$
	
		\begin{aligned}
			c &= q(ab) + r\
			k_a a &= q(ab) + r\
			r &= k_a a - q(ab)\
			r &\equiv 0 quad(\operatorname{mod}\ a)\
			a &\ \ \vert\ \ r
		\end{aligned}&\qquad
		\begin{aligned}
			c &= q(ab) + r\
			k_b b &= q(ab) + r\
			r &= k_b b - q(ab)\
			r &\equiv 0 quad(\operatorname{mod}\ b)\
			b &\ \ \vert\ \ r
		\end{aligned}
	
	$$So $r$ is a common multiple of $a$ and $b$. By [[GCD Times LCM Equal ab]] $\operatorname{lcm}(a,b)=ab/\gcd(a,b)=ab/1=ab$, but $r<ab$ so $r=0$ and $ab$ divides $c$.