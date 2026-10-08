# Transfer from the arc complex and fixed-point corollaries

Use the objects and conventions of [the framework](00-framework.md): $`K=C_1(S_2)`$, its nonseparating subcomplex $`K'`$, and the marked-sphere arc complexes $`A`$ and $`X`$.

## 1. The genus-two action

Birman--Hilden gives the exact sequence
```math
1\longrightarrow\langle\iota\rangle\longrightarrow
\mathrm{Mod}^{+}(S_2)\xrightarrow{\Theta}
\mathrm{Mod}^{+}(S^2,B)\longrightarrow1.
```
See Margalit–Winarski, *The Birman–Hilden Theory*, arXiv:1703.03448v1, printed pp. 1–2, 6. The normal order-two kernel is central. There is an $`\iota`$-invariant model nonseparating curve, the lift of a non-loop arc, and an $`\iota`$-invariant model separating curve, the lift of a $`3|3`$ circle. Surface classification makes each curve type a single mapping-class orbit. Centrality therefore shows that $`\iota`$ fixes every unoriented essential curve class. This proves the class-level assertion needed from target Fact 3.6, printed p. 7; the original Haas–Susskind article is not an independently inspected input here.

If $`f`$ is a fiber-preserving representative of a genus-two mapping class and $`\bar f`$ its quotient, lifting arcs gives
```math
f\Psi(a)=\Psi(\bar f a).
```
Thus the isomorphism of Proposition 6.1 is equivariant for $`\Theta`$. For any $`H\le\mathrm{Mod}^{+}(S_2)`$ and $`\bar H=\Theta(H)`$,
```math
|K'|^H\cong|X|^{\bar H},\qquad |A|^{\bar H}\searrow|X|^{\bar H}.
```
A finite $`F`$ has finite image $`\bar F`$; this image need not be isomorphic to $`F`$.


The arc retraction in this statement is [Theorem E](04-equivariant-arc-retraction.md), with its proof supplied in this repository. The equivariant dictionary is the target Proposition 6.1, pp. 20–21, transported by fiber-preserving representatives; it is not an equivariant strengthening of the full-space Theorem 6.8.

## 2. Exact HOP inputs and identification

We cite Hensel–Osajda–Przytycki, *Realisation and Dismantlability*, **arXiv:1205.0513v1 (2 May 2012)**. The inspected version's Theorem 3.1, printed p. 8, states that a finite subgroup of the mapping class group of a closed oriented marked surface, with negative punctured Euler characteristic on every component, preserves a clique in the arc graph. Definition 2.2, p. 4, makes a clique nonempty; arc cliques are finite (p. 28). Its barycenter is therefore a geometric fixed point. No filling claim is needed from this theorem.

Theorem 10.1, printed pp. 27–28, states that for a closed connected oriented surface with a nonempty marked set and negative punctured Euler characteristic, the geometric fixed-point set of the full arc complex for any subgroup of its mapping class group is empty or contractible. The paragraph following it gives nonempty contractibility for finite subgroups using Theorem 3.1.

Their definitions on p. 7 permit an essential embedded open interval to have equal marked endpoints. Isotopies do not freeze departure directions; their replacement of marks by boundary circles, pp. 8–9, allows proper endpoints to move on the corresponding circles. The arc graph is unoriented and disjointness ignores the marked endpoints. The group preserves the marked set and permits permutations, as also shown by its explicit marked-point-permutation discussion on p. 16; it is orientation preserving. The flag arc complex is defined on p. 27.

For $`(S^2,B)`$, the punctured Euler characteristic is $`2-6=-4`$. A non-loop is automatically essential. A loop is homotopic into its marked basepoint precisely when one side contains no other mark. Single-arc homotopy-isotopy and simultaneous minimal representatives identify their vertices and simplices with $`A`$ of target Definitions 2.3 and 2.5; [Lemma 2.1](02-system-isotopy.md) supplies the common-system identification. Thus it is the full $`A`$, including loops, to which HOP applies, not $`X`$. The fixed sets are geometric ones, including barycenters, with the standard weak realization topology.

## 3. Corollaries

**Corollary FP1.** For every finite subgroup $`F\le\mathrm{Mod}^{+}(S_2)`$, both $`|K'|^F`$ and $`|K|^F`$ are nonempty and contractible.

**Proof.** Its sphere image $`\bar F=\Theta(F)`$ is finite, even if the kernel meets $`F`$. HOP Theorems 3.1 and 10.1 give a nonempty contractible $`|A|^{\bar F}`$. Theorem E strongly deforms this space to $`|X|^{\bar F}\cong|K'|^F`$, making the latter nonempty and contractible. Theorem F in [the comparison file](05-fixed-points-and-obstruction.md) then makes it a strong deformation retract of $`|K|^F`$, which is contractible too. The fixed-link proof also directly covers every finite subgroup fixing a separating vertex, including side exchange. $`\square`$

**Corollary FP2.** For every subgroup $`H\le\mathrm{Mod}^{+}(S_2)`$, each of $`|K'|^H`$ and $`|K|^H`$ is empty or contractible.

**Proof.** HOP Theorem 10.1 and Theorem E give the assertion for $`Z_H=|K'|^H`$. If $`Z_H`$ is nonempty, Theorem F strongly deforms $`|K|^H`$ to it. If it is empty, Theorem F says that $`|K|^H`$ is empty or a single separating vertex. $`\square`$

These two spaces need not be simultaneously empty for an infinite subgroup. The separating stabilizer provides the example. Finite-subgroup fixed-point contractibility does not make the full complex a classifying space for proper actions: its vertex stabilizers include infinite Dehn twist subgroups. No new dismantling theorem or improvement of HOP's arc-complex theorem is asserted.
