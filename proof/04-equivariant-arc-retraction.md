# An equivariant strong deformation retraction of the arc complex

Let $`A,X,B`$ and $`L_S`$ be as in [the arc geometry file](03-arc-cones.md). Set $`G=\mathrm{Mod}^{+}(S^2,B)`$, allowing permutations of $`B`$. Isotopies in this group preserve $`B`$ setwise at every time; their induced permutation is constant, and the identity component fixes $`B`$ pointwise. Thus the action on marked arc classes is well defined. All realizations use the weak CW topology.

**Theorem E.** There is a jointly continuous $`G`$-equivariant strong deformation retraction $`|A|\searrow|X|`$. It restricts to a strong deformation retraction $`|A|^J\searrow|X|^J`$ for every subgroup $`J\le G`$.

## 1. Natural finite cone simplices

For a nonempty all-bad simplex $`S`$ and a regular disjoint representative graph $`\Gamma`$, take all its good faces and define the finite set

```math
Q_{S,\Gamma}=\bigcup_{\Delta\text{ good}}Q(\Delta).
```

This is a set of arc classes, with repetitions removed. Good faces are finite in number; at least one exists; each contributes one or two classes. Every member cones off the whole $`L_S`$ by the proof in [§5](03-arc-cones.md). Since $`L_S`$ is flag, successive adjoining gives

```math
\tau\cup Q_{S,\Gamma}\in L_S\qquad(\tau\in L_S).
```

In particular $`Q_{S,\Gamma}`$ is a nonempty simplex disjoint from the vertex set $`S`$.

For two representatives $`\Gamma,\Gamma'`$ of $`S`$, [Lemma 2.1](02-system-isotopy.md) gives a common ambient isotopy beginning at the identity and fixing all marks. It transports objects, gaps, closure relations, good faces and prescribed unique arc classes. Its terminal homeomorphism acts trivially on arc classes, so the two sets coincide. Write their common value $`Q_S`$.

For $`g\in G`$, transport a representative graph by a smooth representative of $`g`$. The same construction, now permitting marked-point permutations, gives $`Q_{gS}=gQ_S`$. No invariant auxiliary hyperbolic metric is assumed; representative independence removes that choice. Therefore the barycenter

```math
c_S=\frac1{|Q_S|}\sum_{a\in Q_S}e_a
```

satisfies $`c_{gS}=gc_S`$. A stabilizer may permute the vertices of $`Q_S`$ without fixing any one of them; it still fixes $`c_S`$.

## 2. Filtration and attaching blocks

For $`p\ge0`$ define

```math
Y_p=\{\sigma\in A:|\mathrm{bv}(\sigma)|\le p\},\qquad
\mathcal S_p=\{S\in A:|S|=p,\ \mathrm{bv}(S)=S\}.
```

Bad-vertex sets are monotone on faces (target Lemma 8.3, p. 25), so $`Y_p`$ is a subcomplex and $`L_S`$ is a subcomplex. The definitions and the bound in [§6](03-arc-cones.md) give $`Y_0=X`$ and $`Y_{12}=A`$.

If $`|\mathrm{bv}(\sigma)|=p>0`$, let $`S=\mathrm{bv}(\sigma)`$ and $`\tau=\sigma\setminus S`$. Every witnessing bad face lies wholly in $`S`$, so $`\mathrm{bv}(S)=S`$ and $`\tau\in L_S`$. This decomposition is unique (target Lemma 8.6, p. 26).

For $`S\in\mathcal S_p`$, let

```math
B_S=\Delta(S)*L_S,\qquad D_S=\partial\Delta(S)*L_S.
```

These are abstract simplicial joins followed by realization; the boundary includes the empty face. For $`p=1`$, $`D_S=L_S`$. A simplex in $`B_S`$ has the form $`R\sqcup\tau`$ with $`R\subseteq S`$, $`\tau\in L_S`$. Since it is a face of $`S\sqcup\tau`$,

```math
\mathrm{bv}(R\sqcup\tau)\subseteq
\mathrm{bv}(S\sqcup\tau)\cap(R\sqcup\tau)=R.
```

For $`R\subsetneq S`$ it lies in $`Y_{p-1}`$; for $`R=S`$ its bad set is exactly $`S`$. The unique decomposition therefore proves

```math
Y_p=Y_{p-1}\cup\bigcup_{S\in\mathcal S_p}B_S,\qquad
B_S\cap Y_{p-1}=D_S,\qquad
B_S\cap B_T\subseteq Y_{p-1}\quad(S\ne T).
```

The identities also hold on realizations, by the unique finite support of a point.

## 3. Relative mass transfer

For $`x\in|B_S|`$, let $`\lambda_v(x)`$ be its barycentric coordinates, zero off the support, and put $`p=|S|`$. Define

```math
m_S(x)=\min_{s\in S}\lambda_s(x),\qquad
D_t^S(x)=x-tm_S(x)\sum_{s\in S}e_s+ptm_S(x)c_S.
```

Each subtracted coordinate remains nonnegative. The removed mass $`ptm_S(x)`$ is added to the probability vector $`c_S`$, so the total remains one. If the support is $`R\sqcup\tau`$, the image support is contained in the legal simplex $`S\cup\tau\cup Q_S`$. The map starts at $`x`$; at $`t=1`$ at least one $`S`$-coordinate vanishes, so the image lies in $`|D_S|`$. On $`|D_S|`$, a missing $`S`$-coordinate gives $`m_S=0`$, and the whole homotopy is the identity.

On any closed simplex the minimum is a continuous function of finitely many affine coordinates, and the entire simplex prism maps into one finite simplex. Hatcher's closed-cell-prism criterion, printed p. 523, and Theorem A.6, p. 524, give joint continuity for the ordinary product with the compact interval, even without local finiteness. Naturality gives

```math
m_{gS}(gx)=m_S(x),\qquad D_t^{gS}(gx)=gD_t^S(x).
```

## 4. Jointly continuous gluing and restriction

At stage $`p`$, use $`D^S`$ on every block and the identity on $`Y_{p-1}`$. The overlap identities make the map well defined: each block homotopy is the identity on its intersection with the lower layer. Every closed simplex is in that lower layer or a block, so its prism restriction is continuous. The same compact-interval criterion yields a jointly continuous homotopy $`D^{(p)}`$ on $`|Y_p|`$, equivariant because the group permutes the blocks. Its endpoint $`r_p`$ retracts $`Y_p`$ to $`Y_{p-1}`$. If there are no blocks, use the identity.

Put $`R_0=\mathrm{id}_A`$, and $`R_{j+1}=r_{12-j}R_j`$ for $`0\le j\le11`$. For $`t\in[j/12,(j+1)/12]`$ define

```math
D_t(x)=D^{(12-j)}_{12t-j}(R_j(x)).
```

The adjacent time endpoints agree. Finite gluing of the twelve stages gives a jointly continuous equivariant strong deformation retraction onto $`X`$. All stages fix $`X`$ pointwise.

For $`x\in|A|^J`$ and $`j\in J`$, equivariance gives $`jD_t(x)=D_t(jx)=D_t(x)`$. Restriction therefore proves the fixed-space assertion, including empty fixed spaces. These are geometric fixed points, which may lie at barycenters of permuted simplices. The assertion does not replace them by the subcomplex of individually fixed original vertices. $`\square`$
