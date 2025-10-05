---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Category of sets]]"
  - "[[Initial-final object|Final object]]"
---
In $\mathbf{Set}$, any [[Set|Singleton]] is a [[Initial-final object|Final object]].
##### Proof:
Let $A in\text{Obj}(\mathbf{Set})$, a function $f:A -> \{*\}$ can be represented by its [[Function|Graph]] $ Gamma _f subset.eq A times \{*\}\cong A$ such that$$
 forall a in A. exists !b in\{*\}.(a,b) in Gamma _f
$$by there is only such option for $(a,b)$ being $(a,*)$, so the morphism $A\overset{\mathbf{*}}{ -> }\{*\}$ defined by $\mathbf{*}(a)=*$ unique making $\{*\}$ final in $\mathbf{Set}$.