# Arc geometry and cone vertices

## 1. Objects and retained inputs

Let $`B`$ be six marked points on an oriented sphere. Isotopies fix $`B`$ pointwise and do not freeze endpoint directions. Let $`A`$ be the complex of essential unoriented arcs, based loops included, with simplices given by finite collections of distinct classes admitting disjoint interiors. A loop is essential when each of its complementary open discs contains another mark. Let $`X`$ be the flag complex on non-loop classes with adjacency given by disjoint interiors and different unordered endpoint pairs. These are the target paper's Convention 2.1, printed p. 4, and Definitions 2.3–2.5, p. 5.

We retain the following explicitly identified surface facts. Essential single arcs have distinct lifted ideal endpoints, unique simple cusped geodesic representatives in their classes, and these representatives simultaneously realize pairwise minimal interior intersections. For the single-arc facts use Farb–Margalit §1.2.7, pp. 35–36, and Epstein 3.1 and 4.1 in their respective boundary-interval and based-loop settings. The simultaneous-minimum conclusion is the target Theorem 3.13, pp. 10–11: alternating ideal ends force a crossing of any representatives; each geodesic pair crosses at most once in the cover, giving the lower bound for every representative pair. Common geodesics therefore realize all the minima. [Lemma 2.1](02-system-isotopy.md) identifies any two disjoint regular systems with the same component classes by a common marked ambient isotopy.

For the target's Proposition 3.12, pp. 9–10, simplicity must precede the use of homotopy-to-isotopy. An essential arc has distinct ideal ends. The stabilizer of such an unordered end pair in the torsion-free deck group is trivial: a parabolic stabilizer fixes no second point, and an exchanging element would have trivial square. If its geodesic crossed a distinct translate, alternating ends would force the corresponding original embedded lifts to cross, a contradiction. Its radial cusp tails then compactify to an embedded arc or based loop. The cusp conformal smooth structure can be transported to the prescribed smooth marked sphere, as in target Remark 3.3, p. 7. A single-arc isotopy fixing the marks preserves lifted ideal pairs by a uniform cusp-tail cutoff over its compact time interval.

For homotopy-to-isotopy of a non-loop, first cut off cusp tails, retract punctured endpoint discs to their boundaries, and cancel angular endpoint tracks by collar rotations. Epstein 3.1 now applies to proper interval arcs with fixed boundary endpoints. Restore the rotations and fill the discs fixing the centers. For a loop based at $`b`$, use Epstein 4.1 on $`S^2\setminus(B\setminus\{b\})`$; essentiality excludes a bounding disc and orientability excludes a Möbius band. We do not apply the boundary-interval theorem directly to two interior endpoints. The disc uniqueness needed below has its own proof.

## 2. Allowable links

A bad face is a loop vertex or a pair of distinct non-loop vertices having the same endpoint pair. Let $`\mathrm{bv}(\sigma)`$ be the set of vertices in bad faces. For a nonempty all-bad simplex $`S`$, meaning $`\mathrm{bv}(S)=S`$, put

```math
L_S=\{\tau\in\mathrm{lk}_A(S):\mathrm{bv}(S\cup\tau)=S\}.
```

The allowed vertices are precisely the non-loop classes disjoint in the interior from $`S`$ and having no endpoint pair already used by a non-loop member of $`S`$. The subcomplex on these vertices is full in $`X`$ and flag: pairwise admissible classes, together with $`S`$, have common disjoint geodesic representatives. Thus the allowable conditions are vertex conditions. This is the content of target Lemma 10.1, p. 31.

## 3. Existence of good faces

For a regular disjoint representative graph $`\Gamma_S`$, each loop is an object; all non-loop arcs having the same endpoint pair form one object. Each such family has at least two arcs. Distinct objects meet in at most one mark. A gap is a complementary component of an object; it is free when its closure contains no other object. A face is a component of $`S^2\setminus\Gamma_S`$. Call it clean if every pair of distinct boundary marks is an endpoint pair of a non-loop object, and good if it is a clean free gap with one or two interior marks.

We use target Lemmas 9.5–9.11 and Corollaries 9.12–9.13, printed pp. 28–30, in their full statements: object gaps are Jordan discs, with one boundary mark for a loop or two for a parallel-edge object; the boundary marks occur once; nonfree gaps properly contain smaller gaps; minimal gaps are free; and there are two disjoint free gaps, each a face of the whole graph. Each free gap is clean. The finite minimal-gap argument supplies the two disjoint gaps by taking minimal gaps inside two different gaps of any one object.

Each free gap has an interior mark. Otherwise a loop would be inessential, or two bounding arcs of a parallel-edge object would cobound an empty disc and be isotopic. The latter follows by a disc slide in a slightly larger neighborhood of the closed gap, fixing all the marked points. If $`V'`$ marks are touched by $`S`$, the two free gaps satisfy

```math
1\le k(g_1),\quad 1\le k(g_2),\quad
k(g_1)+k(g_2)\le6-V'\le5.
```

Hence one has one or two interior marks and is good (target Lemma 9.15, p. 31). The object/gap inputs are cited from the public target, not supplied by an auxiliary enumeration. [Lemma 2.1](02-system-isotopy.md) transports these gap and boundary properties to every regular representative system of $`S`$.

## 4. Disc-arc uniqueness, with the endpoint repair

**Lemma 3.1.** In a closed Jordan disc, there is one unoriented arc class joining two specified interior marks when they are the only interior marks. There is also one class joining a specified boundary mark to the sole interior mark. In both cases the isotopy fixes the boundary and every mark.

**Proof.** Put two such arcs in finite transverse position with distinct departure directions at their common endpoints, using smooth or PL perturbations fixing the endpoints and boundary. With $`m`$ interior crossings, their union has

```math
V=m+2,\qquad E=2m+2,\qquad F=m+2
```

when viewed on the sphere. Faces have positive even degree. If at most one face were a bigon, then $`2E\ge4F-2`$, contradicting the displayed counts. At most one face contains the outside of the original disc, so there is an interior empty bigon. All marks are endpoints or on the fixed boundary, so its interior contains no mark. For $`m>0`$ its corners cannot both be the original endpoints. A move across its empty disc removes two crossings, or one if an endpoint is a corner; the latter is a rotation about that fixed endpoint. Such moves fix the disc boundary. Continue until $`m=0`$, then slide across the empty disc between the two arcs. In the two-interior-endpoint case the moves have compact support in the disc interior. These moves give an ambient isotopy with the required fixed points. $`\square`$

This proves the needed assertions of target Lemmas 4.9, 10.2 and 10.4 (pp. 16, 32) without treating Epstein's boundary-endpoint theorem as an interior-endpoint theorem.

## 5. Each prescribed arc cones off the whole link

For a good face $`\Delta`$ with one interior mark $`q`$, let $`Q(\Delta)`$ consist of its unique classes from $`q`$ to each boundary mark. For a good face with two interior marks $`q_1,q_2`$, let $`Q(\Delta)`$ contain its unique class $`r`$ joining them. These are classes, not chosen parametrized arcs. Lemma 3.1 proves the uniqueness. Each face contributes one or two classes.

Cleanliness excludes a vertex of $`L_S`$ whose two endpoints are boundary marks of $`\Delta`$: it would either be a loop or have an endpoint pair already present in $`S`$. For one interior mark every allowed arc in the face is a member of the star centered at $`q`$; the one or two star edges have different endpoint pairs and disjoint interiors. Every member of $`Q(\Delta)`$ is therefore adjacent to every other allowed vertex in that face.

For two interior marks choose $`r`$ as above. Given an allowed boundary-to-interior arc $`w`$ ending at $`q_i`$, take a short radial segment at $`q_i`$ in the direction opposite to $`w`$, inside a small disc containing no other mark. The slit disc $`\Delta\setminus w`$ is connected. Join $`q_{3-i}`$ to the far end of that segment by an embedded path in the slit disc, and stop at its first meeting with the segment. The truncated union is an embedded arc joining $`q_1,q_2`$ and meeting $`w`$ only at $`q_i`$. By uniqueness it represents $`r`$. Its endpoint pair differs from that of $`w`$. If the allowed vertex is $`r`$ itself, no extra edge is needed. This supplies the required straightening in target Lemma 10.6, p. 33.

For an allowed vertex $`w`$ in another face, use common geodesic representatives for $`S\cup\{w\}`$; its interior lies in that face. The prescribed arc inside $`\Delta`$ is disjoint from it. A prescribed arc has an interior marked endpoint of $`\Delta`$, untouched by $`S`$, which cannot be an endpoint of an arc in another face. Thus their endpoint pairs also differ. Each prescribed arc belongs to $`L_S`$, and is a cone vertex for its entire vertex set, not only for vertices in $`\Delta`$. Flagness gives

```math
\tau\cup\{a\}\in L_S\qquad(\tau\in L_S,\ a\in Q(\Delta)).
```

This is the repaired cone conclusion of target Lemma 10.8 and Corollary 10.9, p. 34. The representative of a fixed apex class may vary with the tested vertex.

## 6. A finite bound for the whole arc complex

Include all six marks, including isolated ones, in the graph of a simplex of $`A`$. If it has $`E`$ edges, its regular neighborhood has Euler characteristic $`6-E`$. For its complementary compact planar pieces $`R_i`$,

```math
\sum_i\chi(R_i)=E-4,\qquad \sum_i\ell_i=2E,
```

where $`\ell_i`$ counts edge-band sides along boundaries. Non-disc pieces have Euler characteristic at most zero. Every disc piece has $`\ell_i\ge3`$: length one gives an inessential loop; two distinct non-loop edges give an empty bigon; two loops at one basepoint bounding a length-two disc are based homotopic and then isotopic by Epstein 4.1, contradicting distinct classes. A loop and non-loop cannot form a length-two closed walk, and the two sides of a loop lie in different sphere regions. A length-zero piece, or a disc using one non-loop edge twice, would exhaust the sphere with an isolated vertex or edge neighborhood and exclude the other marks. Thus

```math
E-4\le\frac{2E}{3},\qquad E\le12.
```

Consequently every simplex has at most twelve vertices. This supplies the finite bound required from target Lemma 8.5, pp. 25–26, for loops, multiple edges and disconnected systems as well as simple graphs. No classification of maximal simplices is required.
