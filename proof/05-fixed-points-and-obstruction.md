# Fixed points and an equivariance obstruction

Let $`K=C_1(S_2)`$ and let $`K'`$ be its full nonseparating subcomplex. Throughout $`H`$ is a subgroup of $`\mathrm{Mod}^{+}(S_2)`$, unless the extended group is explicitly mentioned. Realizations have the weak CW topology. We use the dictionary of target Proposition 6.1, printed pp. 20–21, and the separating-star geometry of Lemma 6.4 and Corollary 6.5, p. 21, as public inputs.

For a separating curve $`\sigma`$, cutting gives one-holed tori $`T_1,T_2`$. Essential non-boundary-parallel classes in either side are primitive unoriented homology slopes, with intersection $`|ps-qr|`$ (Farb–Margalit, pp. 27, 29, and Proposition 1.10, p. 34). Gluing creates neither new isotopies nor smaller intersections among same-side classes. An isotopy annulus or a bigon cannot contain the essential cut circle: a disc cannot contain it, and an annulus would identify it with its nonseparating core. Thus the slope graph really is the same-side subcomplex in the closed surface. Curves on opposite sides are disjoint. A separating curve has even intersection with every curve, so adjacency to $`\sigma`$ means disjointness. This proves the needed combinatorial part of target Lemma 6.6; the abstract Farey contractibility repair is included below.

## 1. The full-group obstruction

**Theorem O.** No $`\mathrm{Mod}^{+}(S_2)`$-equivariant map $`|K|\to|K'|`$ exists. The same holds for $`\mathrm{Mod}^{\pm}(S_2)`$.

**Proof.** Choose a separating curve class $`\sigma`$ and let
```math
H=\mathrm{Stab}_{\mathrm{Mod}^{+}(S_2)}(\sigma).
```
The source has the $`H`$-fixed point $`e_\sigma`$. We show that the target has no $`H`$-fixed point.

Every $`y\in|K'|`$ has a unique finite nonempty barycentric support
```math
\Omega(y)=\{c:\lambda_c(y)>0\},
```
which is a simplex consisting of nonseparating curve classes. If $`hy=y`$ for every $`h\in H`$, then $`H`$ permutes $`\Omega(y)`$. Each $`c\in\Omega(y)`$ would consequently have finite $`H`$-orbit.

In fact every nonseparating $`c`$ has infinite $`H`$-orbit. If $`i(c,\sigma)>0`$, the Dehn twist $`T_\sigma`$ lies in $`H`$. For $`m\ne n`$, invariance of intersection number and Farb--Margalit Proposition 3.2 give
```math
i(T_\sigma^n c,T_\sigma^m c)
=|n-m|\,i(\sigma,c)^2>0.
```
Thus all the classes $`T_\sigma^n c`$ are distinct.

If $`i(c,\sigma)=0`$, choose representatives disjoint from $`\sigma`$. The curve $`c`$ lies in one of the two one-holed tori $`T_i`$ obtained by cutting along $`\sigma`$. It is not boundary parallel, because $`c`$ is nonseparating. In $`T_i`$ choose an essential curve $`d`$ with $`i(c,d)=1`$: in slope coordinates complete the primitive vector of $`c`$ to an integral basis. They can be drawn with one crossing, and their algebraic intersection is $`\pm1`$ in the corresponding direct summand of $`H_1(S_2)`$, so their geometric intersection in the closed surface is also one. The twist about $`d`$, extended by the identity outside $`T_i`$, fixes $`\sigma`$ and lies in $`H`$. Again
```math
i(T_d^n c,T_d^m c)=|n-m|>0\qquad(n\ne m),
```
so this orbit is infinite as well. The same-side intersection statement is unchanged on the closed surface, by the identification in the opening paragraph.

Both cases contradict the finite orbit forced by an $`H`$-fixed target point. Therefore $`|K'|^H=\varnothing`$. An equivariant map would send $`e_\sigma`$ to an $`H`$-fixed target point, which is impossible. No continuity hypothesis was used. A map equivariant under the extended mapping class group would restrict to an equivariant map under its orientation-preserving subgroup, so it is impossible too. $`\square`$

The twist formula is Farb–Margalit Proposition 3.2, printed p. 69. This theorem rules out an equivariant version of Theorem 6.8, not just equivariance of its particular chosen homotopies.

## 2. Fixed points of the abstract Farey complex

Let $`\mathcal F`$ be the flag complex on primitive unoriented lines in $`\mathbb Z^2`$, with adjacency
```math
[p:q]\sim[r:s]\quad\Longleftrightarrow\quad |ps-qr|=1.
```
It has triangles and no higher simplices. The slope/intersection formula is the target Lemma 6.6, printed pp. 21–22, and Farb–Margalit, printed pp. 27, 29. Its $`\mathrm{PSL}(2,\mathbb Z)`$ action agrees with the usual action on the Farey tessellation.

We use the abstract realization, which includes rational ideal vertices and is **not literally** $`\mathbb H^2`$. Here is its ordinary contractibility proof. Adjacent primitive vectors form a basis, and their only common neighbors are their sum and difference up to sign. Starting outside the triangle with vertices $`0,1,\infty`$, recursively insert mediants in its three boundary intervals. In an endpoint basis an interior rational has coprime positive coordinates $`(m,n)`$; subtracting the smaller from the larger decreases $`m+n`$ and uniquely locates it in the recursion. This exhausts vertices and adjacent triangles. Nested disjoint intervals prevent branch identifications, so the triangle dual is a tree. A finite connected subtree gives a triangle disc, with each leaf adding a new third vertex along its unused side. Every finite subcomplex is contained in such a disc. By Hatcher Proposition A.1, p. 520, compact images lie in finite subcomplexes; sphere maps therefore contract in these discs. Path connectivity and Whitehead's Theorem 4.5, p. 346, give contractibility. Hyperbolic ideal triangles below are used to identify stabilized faces, not to assert a homeomorphism between the two entire spaces.

**Lemma 5.1.** For any $`J\le\mathrm{PSL}(2,\mathbb Z)`$:

- if $`J=1`$, then $`|\mathcal F|^J=|\mathcal F|`$;
- if $`J`$ is finite and nontrivial, $`|\mathcal F|^J`$ consists of one point, an edge midpoint or a triangle barycenter;
- if $`J`$ is infinite, $`|\mathcal F|^J`$ is either empty or a single rational vertex.

Consequently every such fixed space is empty or contractible, and it is nonempty for every finite $`J`$.

**Proof.** First, the pointwise stabilizer in $`\mathrm{PSL}(2,\mathbb Z)`$ of two distinct rational lines is trivial. Indeed, a representative matrix $`M\in\mathrm{SL}(2,\mathbb Z)`$ fixing a primitive integral line sends its primitive generator to $`\epsilon`$ times that generator, with $`\epsilon\in\{1,-1\}`$. For two independent lines, determinant one forces the two signs to agree, so $`M=\pm I`$. It follows that a subgroup preserving a finite set of at least two rational lines embeds in its finite permutation group and is finite.

Suppose now that $`J`$ is finite and nontrivial. It has a common fixed point $`z\in\mathbb H^2`$. An elementary justification is to lift $`J`$ to its finite full inverse image in $`\mathrm{SL}(2,\mathbb R)`$ and average a positive definite quadratic form; after a real change of basis the lifted group is contained in $`\mathrm{SO}(2)`$. A finite-order nonidentity projective matrix cannot fix a rational line: its primitive eigenvector would have eigenvalue $`\pm1`$, and a finite-order such matrix is $`\pm I`$. Thus no vertex of $`\mathcal F`$ is fixed by a nontrivial element of $`J`$.

The point $`z`$ lies in the interior of exactly one Farey ideal triangle or one Farey geodesic edge. That cell is preserved by $`J`$. For an edge, a nontrivial orientation-preserving symmetry must exchange its two endpoints, and the fixed part of the abstract edge is its midpoint. For a triangle, orientation preservation allows only cyclic permutations of its three ideal vertices; a nontrivial stabilizer is of order three, and its fixed part in the abstract triangle is its barycenter. The action on either cell's vertices is faithful by the two-line observation.

There is no second invariant simplex. A nontrivial elliptic isometry has a unique fixed point in $`\mathbb H^2`$. If it preserves a geodesic edge and exchanges the endpoints, that fixed point lies on the edge. If it cyclically permutes a triangle, the fixed point lies inside the ideal triangle: nearest-point projection to this closed convex triangle commutes with the symmetry, so projecting a fixed point outside it would give a second fixed point; a fixed point on its boundary would force a boundary edge to be invariant, which a three-cycle forbids. Disjoint open Farey cells therefore force the same unique cell. Since any fixed abstract point has invariant support, the described midpoint or barycenter is the entire fixed space.

Finally, if $`J`$ is infinite, a fixed point cannot have support of size at least two, by the finite-permutation observation. It must be a rational vertex fixed by every element of $`J`$. There is at most one such vertex, since fixing two would make $`J`$ trivial. If there is one, that vertex is the complete fixed space. The trivial-group case follows from ordinary contractibility. $`\square`$

**Corollary 5.2.** If a subgroup of $`\mathrm{PSL}(2,\mathbb Z)`$ preserves a finite nonempty set of rational slopes, its Farey fixed space is nonempty and contractible. For a singleton, the vertex is fixed; for a larger set, the subgroup is finite and Lemma 5.1 applies. The finite set need not be a Farey simplex.

## 3. Separating links, including exchange of the sides

For a separating $`\sigma`$, let $`T_1,T_2`$ be the one-holed tori. The target Lemma 6.6, printed pp. 21–22, gives
```math
L_\sigma=\mathrm{lk}_K(\sigma)=\mathcal F_1*\mathcal F_2.
```
For a subgroup $`H`$ fixing $`\sigma`$, the subgroup $`N\le H`$ preserving both sides has index one or two. The action on each factor is given by its action on the primitive lines in $`H_1(T_i;\mathbb Z)`$; orientation preservation puts its projective image $`J_i`$ in $`\mathrm{PSL}(2,\mathbb Z)`$. Boundary twists act trivially on these slope vertices. Set
```math
A_i=|\mathcal F_i|^N=|\mathcal F_i|^{J_i}.
```
By Lemma 5.1, each $`A_i`$ is empty, a point, or the whole contractible Farey realization.

If $`N=H`$, an $`H`$-fixed point of the join may have all its mass on one side. Thus $`|L_\sigma|^H`$ is the join of $`A_1`$ and $`A_2`$ when both are nonempty, is the single nonempty $`A_i`$ when the other is empty, and is empty when both are empty. The endpoint cases must not be discarded by a convention in which a topological join with the empty space is empty. These statements follow directly by splitting the barycentric mass into the two vertex sets. We use the CW join topology, equivalently the topology inherited from the abstract simplicial join. Each nonempty case is contractible.

If $`N\ne H`$, choose a side-exchanging $`s\in H`$. An $`H`$-fixed point has equal mass $`1/2`$ on the two sides. There is a homeomorphism
```math
A_1\longrightarrow |L_\sigma|^H,\qquad
x\longmapsto \tfrac12x+\tfrac12sx.
```
Here $`s^2\in N`$ ensures that $`s`$ fixes the displayed point, and $`sNs^{-1}=N`$ ensures that every element of $`N`$ does too. Conversely equal masses and $`s`$-invariance uniquely recover $`x`$ as twice the side-one coordinates. The maps are continuous on the fixed subdivided cells, giving the claimed homeomorphism in the weak topology. In particular the answer is independent of the chosen coset representative $`s`$.

This proves that $`|L_\sigma|^H`$ is always empty or contractible. For finite $`F`$, its side-preserving subgroup has finite projective image on each factor. Both $`A_i`$ are then nonempty, so
```math
|L_\sigma|^F\ne\varnothing\quad\text{and is contractible}.
```
No empty-link example exists for a finite orientation-preserving $`F`$ fixing $`\sigma`$.

## 4. The actual fixed-space attachment, with its topology

Target Lemma 6.4 and Corollary 6.5, printed p. 21, show that a simplex of $`K`$ contains at most one separating vertex. Therefore a fixed point outside $`Z_H=|K'|^H`$ has a unique separating vertex $`\sigma`$ in its support. Support invariance forces $`H`$ to fix that vertex individually. A non-fixed finite orbit of separating vertices cannot contribute a new fixed barycenter: its members do not span a simplex.

It follows, directly from support coordinates, that $`|K|^H`$ is obtained from $`Z_H`$ by adjoining, for each individually $`H`$-fixed separating $`\sigma`$, its fixed star. If $`|L_\sigma|^H`$ is nonempty, the fixed star is its cone with apex $`e_\sigma`$; if the fixed link is empty, the fixed star is just the apex. Distinct fixed stars meet only in their fixed links inside $`Z_H`$. This is a proof of the decomposition, not an assumption that fixed points commute with arbitrary pushouts.

For completeness, these spaces and attaching pairs are CW spaces with the relevant subspace topology. Pass to barycentric subdivision. A simplex there is a chain of nonempty faces of the original complex. A setwise preserved chain has every member individually preserved, since its members have distinct dimensions. Hence the geometric fixed space is precisely the realization of the subcomplex of chains of $`H`$-invariant faces. This observation works for infinite $`H`$ as well. It also identifies fixed links and fixed stars with subcomplexes in the subdivision.

If every attaching fixed link is nonempty and contractible, it is a strong deformation retract of its fixed cone. Indeed both are contractible CW spaces and the inclusion is a subcomplex cofibration; Hatcher Proposition 0.16 and Corollary 0.20 give a retraction homotopy fixing the base. Choose one such homotopy for each fixed star and use the identity on $`Z_H`$. The homotopies agree on overlaps. Every closed fixed cell lies in the core or one star. Applying the closed-cell-prism continuity criterion, with the compact time interval, proves joint continuity of the simultaneous homotopy. Consequently
```math
|K|^H\searrow Z_H
```
in the sense that $`Z_H`$ is a strong deformation retract of $`|K|^H`$.

This conclusion is unconditional whenever all the relevant links are nonempty. In particular it holds for every finite $`F`$, without using HOP. It does not produce one homotopy equivariant under the whole mapping class group: the choices here are made separately on a given fixed space.

## 5. Removing the possible empty-link obstruction for arbitrary subgroups

The following elementary projection argument strengthens the finite-subgroup comparison. It is proved here rather than attributed to HOP.

### Cutting-arc slopes

Fix $`\sigma`$ and consider an essential curve $`c`$ with $`i(c,\sigma)>0`$. Take $`c`$ in minimal position with a fixed representative of $`\sigma`$. Each component of $`c\cap T_i`$ is an essential proper arc in $`T_i`$. If a component were boundary parallel, an innermost such disc would give a bigon between $`c`$ and $`\sigma`$, contradicting minimal position.

An essential proper arc in a one-holed torus is nonseparating and cutting along it yields an annulus: a separating arc would cut off a disc and would be boundary parallel. In the cut annulus choose an embedded path joining the two copies of an interior point of the arc. After gluing, it is a closed curve crossing the arc exactly once. Their algebraic intersection is $`\pm1`$, proving that the relative homology class of the arc is nonzero and primitive. The canonical map
```math
H_1(T_i;\mathbb Z)\longrightarrow H_1(T_i,\partial T_i;\mathbb Z)
```
is an isomorphism: the one boundary circle has zero homology class and $`H_0(\partial T_i)\to H_0(T_i)`$ is an isomorphism in the long exact sequence. Thus the arc determines a primitive unoriented line in $`H_1(T_i)`$, a Farey slope. Equivalently, close the arc through a capped boundary disc and take its essential torus slope. Let $`P_i(c)`$ be the finite set of slopes of these cutting arcs. Both $`P_i(c)`$ are nonempty.

These sets depend only on the curve classes, not on the minimal representatives. To see this, apply Farb--Margalit Lemma 2.9 to the two-curve systems $`(\sigma,c)`$ and $`(\sigma,c')`$. They are essential, nonisotopic, and in minimal position; the triple condition is vacuous for a two-member system. The lemma provides an ambient isotopy taking the first pair to the second, with its terminal map preserving the chosen $`\sigma`$ setwise. This terminal map acts trivially on $`H_1(S_2)`$, and
```math
H_1(S_2;\mathbb Z)=H_1(T_1;\mathbb Z)\oplus H_1(T_2;\mathbb Z).
```
It consequently preserves each summand and acts trivially on it; it cannot exchange the summands. The induced maps on the relative homology groups are also trivial. Hence the cutting arcs give the same slope sets. Lemma 2.9 is on printed pp. 61–62; no multi-curve version with intersecting triples is being assumed.

The same argument using a representative of a mapping class fixing $`\sigma`$ proves naturality. For $`n\in N`$,
```math
P_i(nc)=\rho_i(n)P_i(c),
```
where $`\rho_i`$ is the projective homological action on side $`i`$. A side exchange transports the two sets to one another.

It follows that if $`c`$ crosses $`\sigma`$ and has finite $`N`$-orbit, then
```math
\bigcup_{c'\in N\cdot c}P_i(c')
```
is a finite nonempty $`J_i`$-invariant set of rational slopes. Corollary 5.2 gives $`A_i\ne\varnothing`$ on both sides. Section 3 then gives $`|L_\sigma|^H\ne\varnothing`$, even if $`H`$ exchanges the sides.

### Fixed-space comparison theorem

**Theorem F (fixed-space comparison).** For every $`H\le\mathrm{Mod}^{+}(S_2)`$:

(i) If $`Z_H\ne\varnothing`$, then $`Z_H`$ is a strong deformation retract of $`|K|^H`$.

(ii) If $`Z_H=\varnothing`$, then $`|K|^H`$ is empty or a single separating vertex.

**Proof.** Suppose first that $`Z_H\ne\varnothing`$. Choose a point in it and let $`\Omega`$ be its finite $`H`$-invariant support simplex. For any $`H`$-fixed separating $`\sigma`$, choose $`c\in\Omega`$. If $`i(c,\sigma)=0`$, its finite $`H`$-orbit is a subset of $`\Omega`$ consisting entirely of vertices of $`L_\sigma`$. Its barycenter is therefore an $`H`$-fixed point of $`L_\sigma`$. If $`i(c,\sigma)>0`$, the cutting-arc argument just proved gives a nonempty fixed link instead. Section 3 makes each such fixed link contractible, and Section 4 gives the strong deformation retraction. This proves (i).

If $`Z_H=\varnothing`$, any fixed point with positive nonseparating mass would, by normalizing that mass, give a point of $`Z_H`$. Thus all fixed points are individually fixed separating vertices. There cannot be two distinct such vertices $`\sigma,\sigma'`$. By Lemma 6.4, distinct separating curves cannot be disjoint, so $`i(\sigma,\sigma')>0`$. The $`N`$-orbit of $`\sigma'`$ is a singleton, and the cutting-arc argument would give $`|L_\sigma|^H\ne\varnothing`$. But $`L_\sigma\subset K'`$, contradicting $`Z_H=\varnothing`$. This proves (ii). $`\square`$

The argument uses the actual support simplex, not merely a finite orbit of arbitrary unrelated vertices. This ensures that the barycenter in the zero-intersection case is a legitimate point of the link.


## 6. Scope and examples

For $`H=\mathrm{Stab}(\sigma)`$ the obstruction proof gives $`|K'|^H=\varnothing`$, whereas Theorem F gives $`|K|^H=\{e_\sigma\}`$. This distinguishes empty core fixed spaces from full fixed spaces consisting of a separating vertex.

For $`H=\langle T_\sigma\rangle`$, the twist formula excludes every crossing curve from finite support orbits; the disjoint vertices are fixed. Hence $`|K'|^H=|L_\sigma|`$ and $`|K|^H=|\mathrm{St}(\sigma)|`$. For an orientation-preserving involution exchanging two identical one-holed tori, its fixed link is the diagonal copy of the Farey realization given by the side-exchange formula.

Theorem F gives a separate homotopy on each fixed space. It does not assert a single full-group-equivariant retraction $`|K|\to|K'|`$, which the obstruction excludes. The fixed-space results concern orientation-preserving subgroups; only the mapping obstruction is asserted for the extended group.
