---
tags:
  - theorem
  - category_theory
related topics:
  - "[[Category of sets]]"
  - "[[Initial-final object|Final object]]"
---
In $\mathbf{Set}$, any [[Set|Singleton]] is a [[Initial-final object|Final object]].
##### Proof:
Let $A\in\text{Obj}(\mathbf{Set})$, a function $f:A\to\{*\}$ can be represented by its [[Function|Graph]] $\Gamma_f\subseteq A\times \{*\}\cong A$ such that$$
\forall a\in A.\exists!b\in\{*\}.(a,b)\in\Gamma_f
$$by there is only such option for $(a,b)$ being $(a,*)$, so the morphism $A\overset{\mathbf{*}}{\to}\{*\}$ defined by $\mathbf{*}(a)=*$ unique making $\{*\}$ final in $\mathbf{Set}$.