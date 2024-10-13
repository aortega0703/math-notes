---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Equivalence relation]]"
  - "[[Partition]]"
---
The equivalence classes of an equivalence relation on a set $S$ constitute a partition of $S$. Conversely, for any partition $P$ of $S$, there is an equivalence relation on $S$ whose equivalence classes are the elements of $P$.
##### Proof:
- $\implies$:
	Let $\sim$ be an equivalence relation on $S$. 
	- $x$ is an element of an equivalence class:
		$x\sim x$ for all $x\in S$.
	- $x$ is an element of at most $1$ equivalence class:
		Let $x\in \overline{a}$ and $x\in\overline{b}$, so $a\sim x$ and $b\sim x$, then $a\sim b$ by commutativity and transitivity.
		- $\overline{a} \subseteq \overline{b}$:
			For any $y\in S$, if $a\sim y$ then $b\sim y$ using commutativity and transitivity of $\sim$.
		- $\overline{b} \subseteq \overline{a}$:
			For any $y\in S$, if $b\sim y$ then $a\sim y$ using transitivity of $\sim$.
	- Equivalence classes are non-empty:
		They are defined by an element, so non-empty by definition.
- $\impliedby$:
	Let $x\sim y$ if $\overline{x}=\overline{y}$.
	- Reflexivity:
		$\overline{x}=\overline{x}$ trivially so $x\sim x$.
	- Commutativity:
		Let $x\sim y$. By definition $\overline{x}=\overline{y}$ so $\overline{y}=\overline{x}$ trivially and $y\sim x$.
	- Transitivity:
		Let $x\sim y$ and $y\sim z$. By definition $\overline{x}=\overline{y}$ and $\overline{y}=\overline{z}$ so $\overline{x}=\overline{z}$ trivially and $x\sim y$.