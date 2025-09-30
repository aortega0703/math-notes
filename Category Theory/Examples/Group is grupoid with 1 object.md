---
tags:
  - theorem
  - category_theory
  - math/abstract_algebra
related topics:
  - "[[Group]]"
  - "[[Grupoid]]"
  - "[[Category]]"
---
- For a [[Grupoid]] $\mathcal{C}$ with a single [[Category|Object]] $*$, $(G=\text{Hom}_\mathcal{C}(*,*), \circ)$ is a [[Group]].
- For a [[Group]] $(G,\cdot)$, $\text{Obj}(\mathcal{C})=*$ and $\text{Hom}_\mathcal{C}(*,*)=G$ define a [[Grupoid]] with $\cdot$ as composition.
##### Proof:
- Grupoid $\implies$ group:
	- Closed:
		For any $f,g:*\to *$, $gf: *\to *$.
	- Associative:
		For any $f,g,h:*\to *$, $(hg)f=h(gf)$ by definition of composition in a [[Category]].
	- Has identity:
		For any $f:*\to *$, $f\text{id}_*=\text{id}_*f=f$ by definition of [[Category|Identity morphism]] in a [[Category]].
	- Has inverses:
		For any $f:*\to *$ there exists some $f^{-1}:*\to *$ such that $ff^{-1}=f^{-1}f=\text{id}_*$ by definition of [[Grupoid]].
	Therefore $\text{Hom}_\mathcal{C}(*,*)$ is a group.
- Group $\implies$ grupoid:
	- Identity:
		$e\in G$ by definition of [[Group]], so $\text{id}_*: * \to *$.
	- Composition:
		For $f,g\in G$, $gf\in G$ by definition of [[Group]], so $f,g:*\to*$ implies $gf:*\to*$.
	- Unitality:
		For any $f\in G$, $ef=fe=e$ by definition of [[Group]], so for $f:*\to*$, $\text{id}_*f=f\text{id}_*=\text{id}_*$ in $\mathcal{C}$.
	- Associativity:
		For any $f,g,h\in G$, $(hg)f=h(gf)$ by definition of [[Group]], so for $f,g,h:*\to*$, $(hg)f=h(gf)$ in $\mathcal{C}$.
	Meaning $(*,G,\cdot)$ is a category.
	- Inverses:
		For any $f\in G$, there is some $f^{-1}\in G$ such that $f^{-1}f=ff^{-1}=e$, so for any $f:*\to*$ there is some $f^{-1}:*\to*$ such that $f^{-1}f=ff^{-1}=\text{id}_*$ in $\mathcal{C}$, meaning $f$ is an [[Isomorphism]].
	Therefore $(*,G,\cdot)$ is a grupoid.