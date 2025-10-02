---
tags:
  - theorem
  - math/set_theory
related topics:
  - "[[Equivalence relation]]"
  - "[[Partition]]"
---
For any [[Equivalence relation|equivalence relation]] $\sim$ on a [[Set|set]] $S$, the equivalence classes of $\sim$ constitute a [[Partition|partition]] of $S$. Conversely, for any [[Partition|partition]] $P$ of a [[Set|set]] $S$, there is an [[Equivalence relation|equivalence relation]] on $S$ whose [[Equivalence relation|equivalence classes]] are the elements of $P$.
##### Proof:
- Equivalence relation $\implies$ partition:
	- ${\displaystyle\bigcup_{a in S}} \overline{a}=S$:
		$a in \overline{a}\subseteq S$ for all $a in S$, then $\overline{a} != \emptyset$ and ${\bigcup_{a in S}} \overline{a}=S$.
	- $\overline{a}\cap \overline{b} !=\emptyset$ implies $\overline{a}= \overline{b}$:
		Let $c in a\cap b$, then $a\sim c$ and $b\sim c$, therefore $a\sim b$
		- $\overline{a} \subseteq \overline{b}$:
			Let $a' in \overline{a}$, then $a'\sim a$, so $a'\sim b$ and $a' in \overline{b}$.
		- $\overline{b} \subseteq \overline{a}$:
			Let $b' in \overline{b}$, then $b'\sim b$, so $b'\sim a$ and $b' in \overline{a}$.
		This implies $\overline{a}=\overline{b}$.
- $\impliedby$:
	Let $x\sim y$ when $\overline{x}=\overline{y}$.
	- Reflexivity:
		$\overline{x}=\overline{x}$ trivially so $x\sim x$.
	- Commutativity:
		Let $x\sim y$. By definition $\overline{x}=\overline{y}$ so $\overline{y}=\overline{x}$ trivially and $y\sim x$.
	- Transitivity:
		Let $x\sim y$ and $y\sim z$. By definition $\overline{x}=\overline{y}$ and $\overline{y}=\overline{z}$ so $\overline{x}=\overline{z}$ trivially and $x\sim y$.
