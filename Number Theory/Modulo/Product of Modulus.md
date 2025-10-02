---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Greatest Common Divisor|GCD]]"
  - "[[Congruence under modulo]]"
mathLink: $a\equiv b\ (\operatorname{mod}st)\implies a\equiv b\ (\operatorname{mod}\ s,t)$
---
For $a,b,(s,t>0) in ZZ$
- If $a\equiv b\ (\operatorname{mod}st)$, then $a\equiv b\ (\operatorname{mod}s)$ and $a\equiv b\ (\operatorname{mod}t)$.
- If $a\equiv b\ (\operatorname{mod}s)$, $a\equiv b\ (\operatorname{mod}t)$, and $\gcd(s,t)=1$, then $a\equiv b\ (\operatorname{mod}st)$.
##### Proof:
- $a\equiv b\ (\operatorname{mod}st)\implies a\equiv b\ (\operatorname{mod}s)\land a\equiv b\ (\operatorname{mod}t)$:
	By [[Congruence under modulo]] $st | a-b$ so $s|a-b$ and $t|a-b$.
- $a\equiv b\ (\operatorname{mod}s)\land a\equiv b\ (\operatorname{mod}t)\land\gcd(s,t)=1\implies a\equiv b\ (\operatorname{mod}st)$:
	By [[Congruence under modulo]] $ps = a-b$ and $qt=a-b$ for some $p,q in ZZ$. By [[Division algorithm]] for some $k,(0 lt.eq r < st) in ZZ$$$
	
		a-b &= k(st) + r\
		r &= a-b - k(st)\
		\begin{aligned}
			r &= ps - k(st)\
			&= (p-kt)s\
			s&\ \ |\ r
		\end{aligned}&\qquad
		\begin{aligned}
			r &= qt - k(st)\
			&= (q-ks)t\
			t&\ \ |\ r
		\end{aligned}
	
	$$So $r$ is a common multiple of $s$ and $t$. By [[LCM Divides All Common Multiples]] $r$ is a multiple of $\operatorname{lcm}(s,t)$. By [[GCD Times LCM Equal ab]] $\operatorname{lcm}(s,t)=st$. As $r<st$ then $r=0$ and $st|a-b$, therefore $a\equiv b\ (\operatorname{mod}st)$.