---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Left-right inverse]]"
  - "[[Monic-epic]]"
---
For a [[Category|Morphism]] $g: A\to B$
- if $g$ has a [[Left-right inverse|Left inverse]] it is [[Monic-epic|Monic]].
- if $g$ has a [[Left-right inverse|Right inverse]] it is [[Monic-epic|Epic]].
##### Proof:
- Left inverse $\implies$ Monic:
	Let $f_1, f_2:S\to A$ and $h: B\to A$ such that $gf_1 = gf_2$ and $hg=\operatorname{id}_A$. Then $hgf_1 = hgf_2$ and $f_1=f_2$, so $gf_1 = gf_2 \implies f_1 = f_2$ making $g$ monic.
- Right inverse $\implies$ Epic:
	Let $h_1, h_2: B\to C$ and $f: B\to A$ such that $h_1 g = h_2 g$ and $gf = \operatorname{id}_B$. Then $h_1g f = h_2g f$ and $h_1 = h_2$, so $h_1 g = h_2 g \implies h_1 = h_2$ making $g$ epic.
