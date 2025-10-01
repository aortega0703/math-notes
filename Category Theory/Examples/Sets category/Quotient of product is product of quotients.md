---
tags:
  - theorem
  - category_theory
related topics:
  - "[[Category of sets]]"
  - "[[Product]]"
  - "[[Quotient on set category]]"
---
For [[Equivalence relation|equivalence relations]] $\sim_A$ on $A$ and $\sim_B$ on $B$, and the equivalence relation $\sim$ on $A\times B$ defined by $$
(a_1, b_1) \sim (a_2, b_2)  <==> a_1 \sim_A a_2 \text{ and } b_1 \sim_B b_2.
$$The [[Set operations|Quotient]] $(A\times B)/\!\!\sim$ is [[Isomorphism|isomorphic]] to $(A/\!\!\sim_A)\times(B/\!\!\sim_B)$.
##### Proof:
- There are functions $(A \times B)/\!\!\sim\;\to A/\!\!\sim_A$, $(A \times B)/\!\!∼\;\to B/\!\!\sim_B$:
	![[Quotient of product is product of quotients 1.png]]
	Consider $(a_1,b_1)\sim(a_2,b_2)$, then$$
	
		\pi_{A}\pi_1(a_1,b_1) 
		&= \pi_A (a_1)\
		&= [a_1]\
		&= [a_2]
			&\text{as $(a_1,b_1)\sim(a_2,b_2)\implies a_1\sim a_2$}\
		&= \pi_A (a_2)\
		&= \pi_A \pi_1 (a_2, b_2)
	
	$$So $(a_1,b_1)\sim(a_2,b_2) \implies \pi_A\pi_1(a_1,b_1) = \pi_A\pi_1(a_2,b_2)$ and by [[Quotient on set category]] there exist a unique morphism $\overline{\pi}_A:(A\times B)/\!\!\sim\;\to A/\!\!\sim_A$ such that the diagram commutes (similarly with $B/\!\!\sim_B$).	
- $(A \times B)/\!\!\sim\; \cong (A/\!\!\sim_A) \times (B/\!\!\sim_B)$:
	![[Quotient of product is product of quotients 2.png]]By [[Axiom of choice]] $\pi_A:A\to A/\!\!\sim_A$ has a section $\pi_A': A/\!\!\sim_A\to A$. Then$$
	
		\pi_A' f 
			&= \pi_1 (f\times g)
			&\text{by universality of $A\times B$}\
		\pi_A\pi_A'f &= \pi_A\pi_1(f\times g)\
		f &= \pi_A\pi_1(f\times g)\
		&= \overline{\pi}_A\pi(f\times g)
	
	$$As there is a unique $\pi(f\times g): S\to (A\times B)/\!\!\sim$ that makes the diagram commute (similarly with $B/\!\!\sim_B$), it has the same universal property as the product, so $(A\times B)/\!\!\sim\;\cong (A/\!\!\sim_A)\times (B/\!\!\sim_B)$.