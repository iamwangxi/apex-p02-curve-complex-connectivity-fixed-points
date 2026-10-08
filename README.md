# Higher Connectivity, Fixed Points, and an Equivariance Obstruction for Curve Complexes

[中文说明](README.zh-CN.md)

**Results.** We extend the target paper's simple-connectivity theorem to an explicit higher-connectivity range. In genus two, we prove fixed-space comparison and fixed-point contractibility statements, and show that no map from the full complex to its nonseparating subcomplex can be equivariant under the full orientation-preserving mapping class group, even as a set map.

For integers $`g\ge2`$, $`d\ge1`$, $`k\ge1`$,

```math
d\binom{k+1}{2}\le2g-2\quad\Longrightarrow\quad |C_d(S_g)|\text{ is }k\text{-connected}.
```

In particular $`C_1(S_g)`$ is 2-connected for $`g\ge3`$ and 3-connected for $`g\ge4`$. With $`K=C_1(S_2)`$ and $`K'`$ its full nonseparating subcomplex, every finite $`F\le\mathrm{Mod}^{+}(S_2)`$ has nonempty contractible fixed spaces in both realizations. For every subgroup $`H`$, the two fixed spaces are each empty or contractible; they need not be simultaneously empty. If $`|K'|^H`$ is nonempty, it is a strong deformation retract of $`|K|^H`$; otherwise $`|K|^H`$ is empty or one separating vertex.

## Target and version

Apex Intelligence, [*The Complex of Curves Pairwise Intersecting at Most Once Is Contractible in Genus Two*](https://math.apexin.net/papers/curve-complex-genus-two.pdf), competition PDF dated 11 September 2026, 35 pages, SHA-256 `d1eadd01f94e9af17ee9f5fb2ee1b05b326430f37296309fd9417340ea366fd4`.

This package is v1.0, 8 October 2026. All citations use printed pages and statement identifiers. Theorem H extends target Theorem 1.3, p. 2 (Theorem 7.7, p. 24). The equivariance obstruction gives a boundary for Theorem 6.8, p. 22. Target Proposition 6.1 and its separating-star structure remain cited inputs.

## Reading order

Start with [framework and dependencies](proof/00-framework.md). Then read [higher connectivity](proof/01-higher-connectivity.md), or follow the fixed-point route through [system isotopy](proof/02-system-isotopy.md), [arc cones and repairs](proof/03-arc-cones.md), [the equivariant arc retraction](proof/04-equivariant-arc-retraction.md), [the obstruction and comparison](proof/05-fixed-points-and-obstruction.md), and [HOP transfer and corollaries](proof/06-fixed-point-corollaries.md). [The bibliography](sources/bibliography.md) records the inspected public versions.

The repository includes the full proofs of the three additional ingredients needed for the fixed-point results: representative independence, repaired cone arguments and the equivariant strong deformation retraction. Public classical and target results are cited at their precise scope. No third-party PDFs are redistributed.

## Scope and limits

Theorems concern closed orientable surfaces; the fixed-point conclusions concern orientation-preserving subgroups in genus two. The obstruction also holds for the extended mapping class group by restriction. Theorem H gives a lower bound, not an optimality claim or higher-genus contractibility. Harer Lemma 4.3, pp. 178–179, is a close boundary-replacement and subdivision-homotopy precedent. Souto's unpublished note was not obtained, so higher-connectivity priority is not asserted. Independent novelty and contribution significance remain for expert assessment.

The fixed-point corollaries use Hensel–Osajda–Przytycki Theorems 3.1 and 10.1 in arXiv:1205.0513v1 (2012), applied to the full six-marked-sphere arc complex. The comparison theorem supplies the additional separating-vertex argument for the full curve complex. Individual fixed-space retractions do not form a full-group-equivariant retraction. Infinite vertex stabilizers preclude claiming that the full complex is a model for proper actions on the basis of finite fixed sets.

## Formula format and verification

Inline formulas use GitHub's literal math syntax and display formulas use fenced `math` blocks. All ten Markdown files passed the local GitHub formula-rule check; all 782 formulas also passed a strict local KaTeX 0.16.47 check. Official GitHub rendering remains a publication check. The mathematical proofs have AI adversarial reviews, not a formal proof certificate or human expert certification.

## AI disclosure

GPT-6.1 Sol, in OpenAI Codex under human direction, developed the proof and drafted this text; a separate GPT-6.1 Sol session in a fresh context performed an adversarial review. Claude planned the work, checked key steps against the sources, and reviewed and edited the final text. No human expert has certified the work.

## License

Original prose is licensed under CC BY 4.0; see [LICENSE](LICENSE). External publications retain their own terms. [MANIFEST.sha256](MANIFEST.sha256) identifies every distributed file other than the manifest itself.
