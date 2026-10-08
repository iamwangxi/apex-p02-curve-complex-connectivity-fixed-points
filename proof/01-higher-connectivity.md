# Higher connectivity of intersection-threshold curve complexes

## 1. Statement and conventions

Let $`S_g`$ be a closed connected orientable surface of genus $`g\geq 2`$. A curve is an essential simple closed curve, where essential means that it does not bound a disk. Vertices are unoriented isotopy classes of such curves. Write $`i(a,b)`$ for geometric intersection number, including the convention $`i(a,a)=0`$.

For an integer $`d\geq 0`$, let $`C_d(S_g)`$ be the flag complex on these vertices whose distinct vertices are adjacent when $`i(a,b)\leq d`$. Thus $`C_0(S_g)`$ is the classical curve complex. Geometric realizations have the usual weak topology. For a simplex $`\sigma`$, write $`\#\sigma`$ for its number of vertices and $`|\sigma|`$ for its geometric realization. Write

```math
J:|C_0(S_g)|\longrightarrow |C_d(S_g)|
```

for the inclusion. A space is $`k`$-connected if it is path connected and its homotopy groups in degrees $`1,\ldots,k`$ vanish.

**Theorem H.** Let $`g\geq2`$, $`d\geq1`$, and $`k\geq1`$ be integers. If

```math
d\binom{k+1}{2}\leq 2g-2,
```

then $`|C_d(S_g)|`$ is $`k`$-connected.

In particular, $`C_1(S_g)`$ is $`2`$-connected for $`g\geq3`$, is $`3`$-connected for $`g\geq4`$, and satisfies

```math
\mathrm{conn}\,C_1(S_g)\geq
\left\lfloor\frac{\sqrt{16g-15}-1}{2}\right\rfloor.
```

The principal construction will establish a more specific intermediate statement: the inclusion of every finite subcomplex with sufficiently few intersections in each simplex is homotopic, fixing all its vertices, to a map factoring through $`C_0(S_g)`$.

## 2. A low-intersection system has essential neighborhood boundary

Here and below a regular neighborhood of an embedded finite graph means a compact subsurface containing the graph in its interior and deformation retracting onto it. Such neighborhoods can be taken inside any prescribed open neighborhood of the graph. For completeness, take small disks about the finitely many graph vertices and thin bands along its edges, add thin annuli about any isolated circle components, and round the corners. The disks and bands may all be chosen inside the prescribed open set. No extra components are added.

**Lemma 1 (essential boundary).** Let $`A`$ be a nonempty finite collection of essential embedded circles in $`S_g`$. Suppose intersections are transverse double points, with no triple points, and let $`I`$ be the total number of intersection points in their union $`G`$. If $`I\leq 2g-2`$, every sufficiently small regular neighborhood $`N`$ of $`G`$ has an essential boundary component. The collection and its union need not be connected; different members may be isotopic.

**Proof.** We first compute $`\chi(G)`$ without assuming connectedness or the existence of any intersections. Let $`z`$ be the number of isolated circle components of $`G`$. Give each of these one artificial vertex and one edge. Every intersection vertex has degree four. Consequently

```math
V=I+z,\qquad E=2I+z,\qquad \chi(G)=V-E=-I.
```

The formula also holds when $`I=0`$: the graph is then a disjoint union of circles. Since $`N`$ retracts onto $`G`$,

```math
\chi(N)=-I.
```

Let $`N`$ be any proper regular neighborhood as above. Properness can be ensured by taking the neighborhood sufficiently small, since $`G`$ is a finite embedded graph in a surface. Every connected component of $`N`$ contains at least one of the original essential circles: every component of $`G`$ contains a whole input circle, and the regular neighborhood introduces no new components.

Suppose, for a contradiction, that every component $`\beta`$ of $`\partial N`$ is inessential. On a closed surface of positive genus, $`\beta`$ bounds a unique embedded disk $`D_\beta`$. The interior of the component of $`N`$ incident to $`\beta`$ lies entirely on one side of $`\beta`$. It cannot lie on the disk side, since it contains a circle essential in $`S_g`$, and every embedded circle contained in a disk is inessential in $`S_g`$.

No other component of $`N`$ can lie inside $`D_\beta`$, for the same reason. A connected component of $`N`$ disjoint from $`\beta`$ cannot straddle its two sides. It follows that

```math
\mathrm{int}(D_\beta)\cap N=\varnothing.
```

Thus $`D_\beta`$ is a complementary disk, not merely a disk that may contain other components of the curve system. In particular the disks for different boundary components have disjoint interiors: a nested disk would place a boundary component of $`N`$ inside a disk whose interior misses $`N`$.

Let $`M=\overline{S_g\setminus N}`$. Every component of $`M`$ has nonempty boundary, because $`S_g`$ is connected and $`N`$ is nonempty. For any boundary component $`\beta`$ of such a component, its disk $`D_\beta`$ is exactly that complementary component; one cannot leave its interior through $`\beta`$, which belongs to $`N`$. Hence all components of $`M`$ are disks. If their number is $`F`$, then $`F\geq1`$ because $`N`$ is proper. Additivity of Euler characteristic along boundary circles gives

```math
2-2g=\chi(S_g)=\chi(N)+\chi(M)=-I+F.
```

Therefore $`I=2g-2+F\geq2g-1`$, contradicting the hypothesis. At least one boundary component is essential. $`\square`$

The same count rules out filling: if the curve system filled the closed surface, its regular-neighborhood complement would consist of disks and the displayed equality would again force $`I\geq2g-1`$. The assertion about essential boundary is stronger than merely invoking a non-filling criterion and is proved directly above. The argument accommodates zero-intersection components and disconnected systems throughout.

There is no multiplicity issue in subsequent applications. A vertex denotes a class, and each class receives one representative. If a source map sends several vertices to the same class, that class appears only once in an image simplex. If instead one works with separate parallel representatives of a repeated class, the lemma still applies to their actual double-point count. Coincident copies of one geometric curve are first identified; they are not counted as distinct branches of a graph.

## 3. Simultaneous representatives in general position

**Lemma 2.** For a finite set $`V`$ of distinct vertices of the curve complex, representatives $`a_v`$, $`v\in V`$, can be chosen so that each is embedded, every two intersect in exactly $`i(v,w)`$ transverse points, and no point lies on three representatives.

**Proof.** Give $`S_g`$ a hyperbolic metric and choose the simple closed geodesic representing each class. Distinct simple closed geodesics are simultaneously in pairwise minimal position; see Farb–Margalit, Corollary 1.9 and the paragraph following it, printed p. 33. For essential simple curves, homotopy and isotopy agree by Proposition 1.10, printed p. 34.

Two distinct geodesics cannot have a tangency: equal position and tangent would determine the same geodesic. Their intersections are therefore transverse and finite. There may initially be points at which three or more geodesics pass.

Choose disjoint small disks about these finitely many multiple points. Each incident curve contributes one embedded arc in such a disk, with distinct tangent direction, and each pair of incident arcs has exactly one transverse crossing there. All other parts of the finite family can be kept unchanged.

Here is a concrete local perturbation. In geodesic normal coordinates centered at a multiple point, the incident geodesic arcs are straight lines through the origin. Write their equations as $`\ell_s(x)=0`$, with pairwise independent normal directions. In a smaller concentric disk replace them by $`\ell_s(x)=\varepsilon_s`$. Choose the offsets arbitrarily small and outside the finitely many hyperplanes in offset space which express concurrence of some three lines. Each pair still has exactly one intersection; its position tends to the origin as the offsets tend to zero, so all these intersections can be kept in the smaller disk. Join the shifted arcs smoothly to the original arcs using a cutoff supported in the larger disk, leaving them unchanged near its boundary. The joins can be made arbitrarily small in $`C^1`$. No triple intersection remains in the smaller disk, and sufficiently small joins introduce no intersections in the intervening region.

The pairwise counts remain unchanged. Each original pairwise crossing persists as a unique crossing under sufficiently small $`C^1`$ perturbation, by transversality. Outside small neighborhoods of these crossings, the two compact arcs are separated, so sufficiently small perturbations introduce no new crossing. Embeddedness of each individual arc and curve is preserved as well. Because the family is finite, the perturbations can be made small enough for all these requirements at once. These modifications are isotopies of the individual curves, so their classes remain unchanged. The number of crossings of each pair is still its original geometric intersection number, and hence the new representatives remain pairwise minimal. $`\square`$

The removal of triple points is an elementary local argument supplied here; the cited Farb–Margalit passage supplies simultaneous minimal position, not a separate claim about triple points. At a point incident to $`m`$ distinct curves, the perturbation creates $`\binom m2`$ distinct double points in place of the multiple point, preserving the contribution to each pairwise count. It does not assert preservation of the number of distinct geometric points before the perturbation.

## 4. A compatible finite replacement

**Proposition 3 (finite replacement).** Let $`L\subseteq C_d(S_g)`$ be a finite subcomplex. Choose the representatives of its vertex set as in Lemma 2. Assume that for every nonempty simplex $`\sigma\in L`$,

```math
I_\sigma:=\sum_{\{v,w\}\subseteq\sigma}i(v,w)\leq2g-2.
```

There exist a simplicial map

```math
r:\mathrm{sd}\,L\longrightarrow C_0(S_g)
```

and a homotopy, fixed on every vertex of $`L`$,

```math
u\simeq J\circ |r|\circ h_L^{-1},
```

where $`u:|L|\hookrightarrow |C_d(S_g)|`$ is the inclusion and $`h_L:|\mathrm{sd}\,L|\to |L|`$ is the canonical subdivision homeomorphism.

**Proof.** We construct all choices on the image subcomplex $`L`$ itself, so a shared face receives one choice regardless of which coface or source simplex contains it.

### 4.1. Nested neighborhoods

For a nonempty simplex $`\sigma`$, let

```math
G_\sigma=\bigcup_{v\in\sigma}a_v.
```

After Lemma 2 its actual double-point count is $`I_\sigma`$. For each such simplex choose a proper compact regular neighborhood $`N_\sigma`$ with $`G_\sigma\subset\mathrm{int}(N_\sigma)`$, requiring

```math
\tau\subsetneq\sigma\quad\Longrightarrow\quad
N_\tau\subset\mathrm{int}(N_\sigma).
```

These choices exist by descending induction on simplex dimension. After all strict cofaces of $`\tau`$ have been treated, the finite intersection

```math
U_\tau=\bigcap_{\substack{\sigma\in L\\\tau\subsetneq\sigma}}
\mathrm{int}(N_\sigma)
```

is an open neighborhood of $`G_\tau`$: the common representatives give $`G_\tau\subseteq G_\sigma\subset\mathrm{int}(N_\sigma)`$ for every coface. If there is no strict coface, take $`U_\tau=S_g`$. The elementary regular-neighborhood construction in Section 2 gives $`N_\tau\subset U_\tau`$. Only finitely many cofaces are involved. No compatibility between incomparable faces is required.

By Lemma 1 choose an essential boundary component $`c_\sigma\subset\partial N_\sigma`$ for each nonempty $`\sigma`$. For a singleton $`\sigma=\{v\}`$, $`N_\sigma`$ is an annulus about $`a_v`$, and either boundary component represents $`v`$. Thus

```math
[c_{\{v\}}]=v.
```

### 4.2. The subdivision map

A vertex of $`\mathrm{sd}\,L`$ is a nonempty simplex $`\sigma`$ of $`L`$. Define

```math
r(\sigma)=[c_\sigma].
```

A simplex of $`\mathrm{sd}\,L`$ is a strict inclusion chain $`\sigma_0\subsetneq\cdots\subsetneq\sigma_m`$. For $`a<b`$, the curve $`c_{\sigma_a}`$ lies in $`N_{\sigma_a}\subset\mathrm{int}(N_{\sigma_b})`$, whereas $`c_{\sigma_b}`$ lies on its boundary. These actual representatives are disjoint. Thus the distinct classes in the list $`[c_{\sigma_0}],\ldots,[c_{\sigma_m}]`$ span a simplex of $`C_0(S_g)`$. This defines a simplicial map, including when some of the classes coincide: a simplicial map may collapse a simplex to a lower-dimensional simplex.

### 4.3. Cone carriers

For each nonempty $`\sigma\in L`$, form the finite vertex set

```math
W_\sigma=\sigma\ \cup\ 
\{[c_\tau]:\varnothing\neq\tau\subseteq\sigma\}
```

and let $`P_\sigma`$ be the full subcomplex of $`C_d(S_g)`$ spanned by $`W_\sigma`$. Let $`b_\sigma=[c_\sigma]`$.

The vertex $`b_\sigma`$ has intersection number zero with every vertex of $`W_\sigma`$. It is disjoint from all $`a_v`$ for $`v\in\sigma`$, since these curves lie in $`\mathrm{int}(N_\sigma)`$. For a proper face $`\tau`$ of $`\sigma`$, it is disjoint from $`c_\tau`$ by nesting. Equality of classes causes no problem because $`i(b_\sigma,b_\sigma)=0`$.

Since $`C_d(S_g)`$ is flag and $`P_\sigma`$ is full, every simplex $`\eta`$ of $`P_\sigma`$ extends to the simplex $`\eta\cup\{b_\sigma\}`$. Consequently $`P_\sigma`$ is a simplicial cone with apex $`b_\sigma`$. In particular its realization is contractible; its contraction is the linear contraction of each point to $`b_\sigma`$ inside the enlarged simplex.

This does **not** assert that all the other vertices of $`W_\sigma`$ span a simplex. Curves associated to incomparable faces may intersect more than $`d`$. The cone assertion needs only a universal adjacent apex and the flag property.

Also, if $`\tau\subseteq\sigma`$, then $`W_\tau\subseteq W_\sigma`$, and fullness gives

```math
P_\tau\subseteq P_\sigma.
```

Set $`q=J\circ |r|\circ h_L^{-1}`$. The map $`u`$ sends $`|\sigma|`$ into $`|P_\sigma|`$, because its vertices are in $`\sigma`$. The map $`q`$ sends $`|\sigma|`$ into $`|P_\sigma|`$, because the subdivision of $`\sigma`$ uses only vertices corresponding to its nonempty faces. For a vertex $`v`$, both maps take the value $`v`$, and $`P_{\{v\}}`$ is the single point $`v`$.

### 4.4. An explicit relative carrier argument

We construct $`H:|L|\times[0,1]\to |C_d(S_g)|`$ such that

```math
H(-,0)=u,\qquad H(-,1)=q,\qquad
H(|\sigma|\times[0,1])\subseteq |P_\sigma|.
```

On each vertex prism set $`H(v,t)=v`$ for all $`t`$. Suppose the homotopy has already been constructed on prisms over all proper faces of an $`m`$-simplex $`\sigma`$, with $`m\geq1`$. On

```math
B_\sigma=(|\sigma|\times\{0,1\})\ \cup\ 
(|\partial\sigma|\times[0,1])
```

we have a well-defined continuous map: use $`u`$ at the bottom, $`q`$ at the top, and the already constructed face homotopies on the sides. The maps agree on intersections because the face homotopies have those prescribed endpoints and were constructed once for each face. The whole boundary map lands in $`|P_\sigma|`$, since every proper-face carrier is a subcomplex of $`P_\sigma`$.

The prism $`|\sigma|\times[0,1]`$ is a closed $`(m+1)`$-ball with boundary $`B_\sigma`$. Its boundary map extends to this ball using the cone contraction of $`|P_\sigma|`$. More explicitly, identify the prism with the cone on its boundary by choosing an interior point and using radial segments. On a segment from a boundary point $`x`$ to this interior point, map the segment to the cone segment from the prescribed value $`H(x)`$ to $`b_\sigma`$. The apex condition guarantees that this segment lies in $`|P_\sigma|`$; the result is continuous, including at the interior point. It retains the previously assigned map on the entire boundary.

Do this for each $`m`$-simplex and continue in increasing dimension. Two same-dimensional simplex prisms intersect only in prisms over their common faces, where the map has already been fixed. The finite gluing produces a continuous homotopy on $`|L|\times[0,1]`$. Its vertex restrictions are the original constant homotopies. This proves the proposition. $`\square`$

Only the explicitly exhibited finite cones $`P_\sigma`$ were used to extend the homotopy. No assertion about contractibility or connectivity of a link in $`C_d(S_g)`$ is involved. Nor is the construction a global retraction of $`C_d`$ onto $`C_0`$: it depends on the chosen finite subcomplex.

## 5. Closing the genus-three case first

Consider $`g=3`$, $`d=1`$, $`k=2`$. A simplex in a $`2`$-dimensional subcomplex of $`C_1(S_3)`$ has at most three distinct vertices. With the simultaneous representatives above, its intersection count is at most

```math
\binom32=3\leq4=2g-2.
```

Hence Proposition 3 applies to every finite subcomplex of dimension at most two.

Fix a vertex $`v_0`$ as basepoint. For $`j=1`$ or $`2`$, let $`f:(S^j,*)\to(|C_1(S_3)|,v_0)`$ be any continuous based map. Triangulate $`S^j`$ finitely with $`*`$ a vertex. The simplicial approximation theorem gives, after subdivision, a simplicial approximation $`f_0`$ and a homotopy from $`f`$ to $`f_0`$ fixed at $`*`$; the fixed-vertex assertion is stated explicitly after Hatcher's Theorem 2C.1, printed p. 179.

Let $`L`$ be the union of the image simplices of $`f_0`$ and their faces. Then $`L`$ is finite and has dimension at most $`j\leq2`$, even if $`f_0`$ identifies some source vertices. It is important to take this union, rather than the full subcomplex on all image vertices, which could have much higher dimension.

Proposition 3 homotopes the inclusion $`u:|L|\to |C_1(S_3)|`$, fixing $`v_0`$, to $`J\circ |r|\circ h_L^{-1}`$. Consequently $`f`$ is based homotopic to $`J\circ a`$, where

```math
a=|r|\circ h_L^{-1}\circ f_0:S^j\to |C_0(S_3)|
```

is a based map. Harer's theorem gives that $`C_0(S_3)`$ is $`3`$-connected, so $`a`$ is based null-homotopic for $`j=1,2`$. Composing that null-homotopy with $`J`$ shows that $`f`$ is based null-homotopic.

Finally $`C_1(S_3)`$ is path connected: $`C_0(S_3)`$ is path connected and contains all vertices, and every point of $`C_1(S_3)`$ can be joined within its simplex to a vertex. Thus $`C_1(S_3)`$ is $`2`$-connected. This proves the genus-three case with a homotopy compatible on shared faces.

## 6. General parameters

Harer's *The Cohomology of the Moduli Space of Curves* supplies the classical input

```math
|C_0(S_g)|\simeq\bigvee S^{2g-2}.
```

Its complex $`Z_g^0`$, defined on printed p. 170, uses all nontrivial mutually non-isotopic disjoint curves, including separating curves. On a closed surface, simultaneous minimal representatives and homotopy-isotopy equivalence identify this with $`C_0(S_g)`$. Lemma 3.6, p. 171, identifies it with $`\partial W`$ up to homotopy; Theorem 4.1, p. 176, gives the sphere dimension $`2g-2`$ for $`s=0`$. Hence $`C_0(S_g)`$ is $`(2g-3)`$-connected. These are statements from the inspected expository chapter.

**Proof of Theorem H.** First check that the proposed range is within Harer's range. If $`k=1`$, then $`k\leq2g-3`$ because $`g\geq2`$. If $`k\geq2`$, then

```math
k+1\leq\binom{k+1}{2}\leq
d\binom{k+1}{2}\leq2g-2,
```

so again $`k\leq2g-3`$.

Fix $`1\leq j\leq k`$ and an arbitrary based map $`f:S^j\to |C_d(S_g)|`$ with a vertex basepoint. Take a based simplicial approximation $`f_0`$ as in Section 5, and let $`L`$ be its finite image subcomplex, consisting of its image simplices and their faces. Then $`\dim L\leq j`$.

For any nonempty simplex $`\sigma`$ of $`L`$, its distinct vertices are at most $`j+1`$ in number, and the definition of $`C_d`$ gives

```math
I_\sigma=\sum_{\{v,w\}\subseteq\sigma}i(v,w)
\leq d\binom{\#\sigma}{2}
\leq d\binom{j+1}{2}
\leq d\binom{k+1}{2}
\leq2g-2.
```

Proposition 3 thus gives a based homotopy of $`f`$ to $`J\circ a`$ for a based map $`a:S^j\to|C_0(S_g)|`$. Since $`j\leq k\leq2g-3`$, Harer's theorem supplies a based null-homotopy of $`a`$. Its composite with $`J`$ is a based null-homotopy of $`J\circ a`$, and concatenation shows that $`f`$ represents zero in $`\pi_j(|C_d(S_g)|,v_0)`$.

The target is path connected by the same argument as in Section 5, using that $`C_0`$ contains all its vertices. Vanishing at a vertex basepoint therefore gives vanishing at any basepoint. This proves $`k`$-connectivity. $`\square`$

Equivalently, Proposition 3 shows that $`J`$ is surjective on $`\pi_j`$ for every $`j`$ in the displayed intersection range. This surjectivity follows from a homotopy fixed at the basepoint, rather than merely from an unbased replacement.

For $`d=1`$, solving $`k(k+1)/2\leq2g-2`$ gives exactly the stated floor bound. At $`g=3`$ it gives $`k=2`$; at $`g=4`$ it gives $`k=3`$; at $`g=6`$ it gives $`k=4`$. No new geometric hypothesis was introduced in passing from the genus-three construction to general parameters.


## 7. Relation to the target and method precedent

For $`d=1,k=1`$, Theorem H recovers the target paper's Theorem 1.3, printed p. 2, proved as Theorem 7.7, p. 24. For general $`d`$, the $`k=1`$ case gives $`d\le2g-2`$. The additional argument is Proposition 3's coherent replacement of finite higher-dimensional images, including a homotopy fixing their common faces and vertices.

Harer's Lemma 4.3, printed pp. 178–179, is a close method precedent. Its proof replaces possibly intersecting curve systems by essential regular-neighborhood boundaries on a subdivision and constructs a homotopy. The present use of nested finite neighborhoods and full cone carriers applies that method to the intersection-threshold complex with the explicit Euler bound. The numerical theorem is not attributed to Harer Lemma 4.3 itself.

The target paper, printed p. 2, reports that Souto stated Theorem 1.3 without proof. Souto's unpublished note has not been obtained; no assertion is made about whether it states higher connectivity. Neither independent novelty nor optimality of the bound has been established. Theorem H does not establish higher-genus contractibility.

See [the bibliography](../sources/bibliography.md) for versions and printed-page locators.
