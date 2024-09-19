---
tags:
  - theorem
  - abstract_algebra
related topics:
  - "[[Group]]"
  - "[[Order]]"
mathLink: $ab=ba \implies |ab|$ divides $|a||b|$
---
For a finite [[Group]] $G$ and $a,b\in G$, if $ab=ba$ then $|ab|$ divides $|a||b|$.
##### Proof:
Using the hypothesis one can obtain $(ab)^{|a||b|} = a^{|a||b|}b^{|a||b|}$ by reordering terms. Then by [[Order divides exponent]] $a^{|a||b|}b^{|a||b|} = e$, so also by [[Order divides exponent]] $|ab|$ divides $|a||b|$.