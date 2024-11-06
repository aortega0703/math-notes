---
tags:
  - theorem
  - abstract_algebra
related topics:
  - "[[Order]]"
---
For an [[Abelian group]] $G$, if $g$ is has maximal finite order (i.e. $|g|\geq |h|$ for all $h\in G$) then $|h|$ divides $|g|$ for all $h\in G$.
##### Proof:
Suppose $|h|$ does not divide $|g|$, then by [[If not divides then has a prime exponent greater]] there is some prime $p$ such that $|h|=p^ns$ and $|g|=p^mr$ with $r$ and $s$ relatively prime to $p$ and $m < n$.
- $|g^{p^m}|=r$:
	By [[Order of power element]] $|g^{p^m}|=|g|/\gcd(|g|,p^m)=|g|/p^m=r$.
- $|h^s|=p^n$:
	By [[Order of power element]] $|h^s|=|h|/\gcd(|h|,s)=|h|/s=p^n$.
By [[Elements commute implies order of product]] $|g^{p^m} h^s|=r p^n>r p^m=|g|$. This is a contradiction as $|g|$ is an element of maximal order, so $|h|$ must divide $|g|$.