---
tags:
  - theorem
  - math/set_theory
  - needs_details
related topics:
  - "[[Set]]"
  - "[[Subset]]"
  - "[[Power set]]"
  - "[[Cardinality]]"
---
For a set $S$ with $|S|=n$, $|\mathcal{P}(S)|=2^n$.
##### Proof:
- Case $n=0$:
	If $|S|=0$ then $S=\emptyset$, whose only subset is itself. Therefore $|\emptyset|=2^0=1$.
- Case $n+1$:
	Let $S$ be a set with $|S|=n+1$ and $s in S$. By $|S-\{s\}| = n$ so by induction $\big|\mathcal{P}(S-\{s\})\big| = 2^n$. Let $A$ be the subsets of $S$ that do not contain $s$ and $B=$ the subsets of $S$ that do. Note that $A\cup B=\mathcal{P}(S)$ and $A\cap B = \emptyset$.
	- $\big|A\big|  lt.eq \big|B\big|$:
		If $T in A$, then $T in \mathcal{P}(S)$ with $s\notin T$. So $T \cup \{s\} \subseteq S$, therefore $T\cup \{s\}  in B$.
	- $\big|B\big|  lt.eq \big|A\big|$:
		If $T in B$, then $T in \mathcal{P}(S)$ with $s in T$. So $T - \{s\} \subseteq S$, therefore $T- \{s\}  in B$.
	So $\big|A\big| = \big|B\big|$. Therefore $\big|\mathcal{P}(S)\big|$ $= \big|A\big| + \big|B\big|$ $=2 \big|A\big|$ $= 2 (2^n)$ $= 2^{n+1}$.
Therefore $|\mathcal{P}(S)|=2^n$ as intended.
