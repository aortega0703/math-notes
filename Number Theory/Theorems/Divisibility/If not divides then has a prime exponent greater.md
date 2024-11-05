---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Divisibility]]"
---
For $n,m\in\mathbb{Z}^+$, if $n$ does not [[Divisibility|divides]] $m$ then there is a [[Divisibility|Prime]] $p$ such that $n=p^a r$ and $m=p^b s$ with $r,s$ both relative primes to $p$ and $a>b$.
##### Proof:
By [[GCD Factors Into Relative Primes]] $n=\gcd(n,m)r$ and $m=\gcd(n,m)s$ with $r,s$ relative primes to each other. If $r=1$ then $m=ns$ which is a contradiction as $n$ does not divide $m$, so $r>1$. By [[Fundamental theorem of arithmetic]] $r$ is a product of primes, let $p$ be any one of them and $a>0$ such that $r=p^a r'$ with $r'$ relative prime with $p$. Let $b\geq 0$ such that $\gcd(n,m)= p^b g$ with $g$ relative prime with $p$. Then $n=p^{a+b}gr'$ and $m=p^bgs$. Clearly $a+b>b$ and by [[Relative Prime with Product]] $gr'$ and $gs$ are both relative primes with $p$, which concludes the proof.