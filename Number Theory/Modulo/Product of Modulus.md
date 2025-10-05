---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Greatest Common Divisor|GCD]]"
  - "[[Congruence under modulo]]"
mathLink: $a\equiv b\ (op("mod")st) ==> a\equiv b\ (op("mod")\ s,t)$
---
For $a,b,(s,t>0) in ZZ$
- If $a\equiv b\ (op("mod")st)$, then $a\equiv b\ (op("mod")s)$ and $a\equiv b\ (op("mod")t)$.
- If $a\equiv b\ (op("mod")s)$, $a\equiv b\ (op("mod")t)$, and $\gcd(s,t)=1$, then $a\equiv b\ (op("mod")st)$.
##### Proof:
- $a\equiv b\ (op("mod")st) ==> a\equiv b\ (op("mod")s)\land a\equiv b\ (op("mod")t)$:
	By [[Congruence under modulo]] $st | a-b$ so $s|a-b$ and $t|a-b$.
- $a\equiv b\ (op("mod")s)\land a\equiv b\ (op("mod")t)\land\gcd(s,t)=1 ==> a\equiv b\ (op("mod")st)$:
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
	
	$$So $r$ is a common multiple of $s$ and $t$. By [[LCM Divides All Common Multiples]] $r$ is a multiple of $op("lcm")(s,t)$. By [[GCD Times LCM Equal ab]] $op("lcm")(s,t)=st$. As $r<st$ then $r=0$ and $st|a-b$, therefore $a\equiv b\ (op("mod")st)$.