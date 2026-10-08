# Framework, results and dependency map

All surfaces in the higher-connectivity theorem are closed, connected and orientable. Curves are essential unoriented simple closed curve isotopy classes; separating classes are included. The complexes $`C_d(S_g)`$ are flag complexes with adjacency $`i(a,b)\le d`$. All realizations have the weak CW topology. A $`k`$-connected space is path connected with vanishing homotopy groups through degree $`k`$.

In genus two, $`K=C_1(S_2)`$ and $`K'`$ is its full nonseparating subcomplex. Let $`B`$ be the six hyperelliptic branch points; $`A`$ is the full essential arc complex, loops included, and $`X`$ is the non-loop subcomplex with the different-endpoint-pair adjacency condition. $`X`$ is not full in $`A`$. Mapping classes are orientation preserving, and marked points may be permuted. Isotopies starting at the identity fix every mark pointwise. Fixed spaces always mean geometric fixed spaces, not complexes of individually fixed original vertices.

The full proofs follow this dependency order:

| Result or input | Proof supplied here | Public inputs retained |
|---|---|---|
| Theorem H: $`d\binom{k+1}{2}\le2g-2`$ implies $`k`$-connectivity | [01](01-higher-connectivity.md): Euler boundary lemma, simultaneous general-position representatives, nested neighborhoods, finite cone carriers and based homotopy | Farb–Margalit Corollary 1.9 and Proposition 1.10; Hatcher 2C.1; Harer 3.6 and 4.1 |
| Representative independence for disjoint arc systems | [02](02-system-isotopy.md): cyclic order, integral cusp winding, truncation and common isotopy | Classical single-arc hyperbolic and isotopy facts; Epstein 3.1/4.1; Farb–Margalit 2.9 |
| Good-face arcs cone off every allowable link | [03](03-arc-cones.md): endpoint repair, full-link argument, and twelve-vertex bound for $`A`$ | Target object/gap Lemmas 9.5–9.11 and Corollaries 9.12–9.13; canonical arc representatives |
| Theorem E: $`\lvert A\rvert\searrow\lvert X\rvert`$ equivariantly | [04](04-equivariant-arc-retraction.md): natural finite cone simplex, mass transfer, block gluing and fixed-space restriction | 02 and 03; target bad-vertex definitions; Hatcher's product-prism criterion |
| Obstruction and Theorem F: fixed-space comparison | [05](05-fixed-points-and-obstruction.md): orbit argument, Farey contractibility and fixed-point classification, cutting slopes and CW gluing | Target 6.4–6.5; one-holed-torus slopes; Farb–Margalit 2.9 and 3.2; Hatcher 0.16/0.20/A.1/A.6/4.5 |
| FP1 and FP2 | [06](06-fixed-point-corollaries.md): equivariant dictionary, HOP interface and deduction | Theorems E and F; target Proposition 6.1; Birman–Hilden; HOP 3.1 and 10.1 |

This is self-contained at the level of the cited public mathematical statements: all additional arc-retraction, cone-repair and system-isotopy arguments needed for the fixed-point deductions are included. Classical surface topology, Harer's theorem, the target's full hyperelliptic dictionary and HOP remain explicitly cited inputs.

The target paper's ordinary strong deformation retraction (Theorem 6.8, p. 22) provides a comparison, not a full-group-equivariant input. The obstruction shows that such an equivariant map cannot exist. Theorem F instead supplies a separately chosen strong deformation retraction on each nonempty-core fixed space.

Theorem H extends target Theorem 1.3 (p. 2; Theorem 7.7, p. 24). It neither strengthens the target's genus-two ordinary contractibility to higher-genus contractibility nor claims the bound optimal. Harer Lemma 4.3 is an explicit method precedent. No worldwide novelty or prize-level assessment follows from the proofs.
