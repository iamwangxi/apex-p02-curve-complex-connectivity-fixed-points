# 曲线复形的高阶连通性、不动点与等变映射障碍

[English](README.md)

**结论。** 对闭、连通、可定向曲面和整数 $`g\ge2,d\ge1,k\ge1`$，

```math
d\binom{k+1}{2}\le2g-2\ \Longrightarrow\ |C_d(S_g)|\text{ 为 }k\text{-连通空间}.
```

特别地，$`g\ge3`$ 时 $`C_1`$ 为 2-连通，$`g\ge4`$ 时为 3-连通。亏格二中，令 $`K=C_1(S_2)`$、$`K'`$ 为完整非分离子复形：不存在 $`\mathrm{Mod}^{+}(S_2)`$ 等变映射 $`|K|\to|K'|`$，连集合映射也不存在。每个有限保向映射类子群在两个空间上的不动点集均非空可缩；任意子群的不动点集各自为空或可缩。核心不动点集非空时，完整不动点空间强形变收缩到核心；核心为空时，完整空间为空或一个分离顶点。

## 对象与版本

目标为 Apex Intelligence 的 [*The Complex of Curves Pairwise Intersecting at Most Once Is Contractible in Genus Two*](https://math.apexin.net/papers/curve-complex-genus-two.pdf)，2026-09-11 比赛版，35 页，PDF SHA-256 `d1eadd01f94e9af17ee9f5fb2ee1b05b326430f37296309fd9417340ea366fd4`。本包版本 v1.0，2026-10-08；引用均使用印刷页码和定理编号。

定理 H 是论文 Theorem 1.3（第 2 页，正文 Theorem 7.7，第 24 页）的高阶推广。映射障碍说明 Theorem 6.8（第 22 页）的普通收缩不能具有完整映射类群等变性。Proposition 6.1 与论文分离星结构仍作为公开引用输入。

## 文件导览与证明边界

先读[框架与依赖](proof/00-framework.md)。连通性路线见[完整证明](proof/01-higher-connectivity.md)。不动点路线依次为[系统同痕](proof/02-system-isotopy.md)、[弧与锥修补](proof/03-arc-cones.md)、[等变弧收缩](proof/04-equivariant-arc-retraction.md)、[障碍与固定点比较](proof/05-fixed-points-and-obstruction.md)、[HOP 接口与推论](proof/06-fixed-point-corollaries.md)。[书目](sources/bibliography.md)记载实际核对的公开版本。

系统同痕、锥修补和等变强形变收缩的所需证明全部收录。经典单弧理论、Harer、Birman–Hilden、HOP 与论文的指定陈述按准确范围引用，不声称重证全部经典理论。不打包第三方 PDF。

高阶连通界未证明最优，也未得到高亏格可缩性。Harer Lemma 4.3（第 178–179 页）已有非常接近的边界替换、细分和同伦先例。未取得 Souto 未发表笔记，不主张更高连通性从未被陈述。独立新颖性与贡献价值待专家评估。

不动点可缩性使用 HOP 的 arXiv:1205.0513v1（2012-05-02）Theorems 3.1、10.1，先应用到含 loop 的完整六标点球面弧复形，再借本包比较定理处理分离顶点。固定点结果限保向子群；扩展映射类群只得到映射障碍。不同无限子群下两个空间未必同时为空。分别在固定点空间上的收缩不构成完整群等变收缩。顶点稳定子无限，因此有限子群不动点可缩不推出本复形是 proper-action 分类空间。

## 公式与核验

行内公式使用 GitHub 原样数学语法，独立公式使用 `math` 围栏。10 个 Markdown 文件均已通过本地 GitHub 公式规则检查，782 条公式通过 KaTeX 0.16.47 严格检查。GitHub 官方渲染仍须在发布前检查。已有 AI 数学对抗复核，不等于形式化证明或人类专家认证。

## AI 声明

GPT-6.1 Sol, in OpenAI Codex under human direction, developed the proof and drafted this text; a separate GPT-6.1 Sol session in a fresh context performed an adversarial review. Claude planned the work, checked key steps against the sources, and reviewed and edited the final text. No human expert has certified the work.

## 许可

原创散文部分采用 CC BY 4.0，见 [LICENSE](LICENSE)。第三方文献保留其各自权利。[MANIFEST.sha256](MANIFEST.sha256)列出除清单自身外全部分发文件的指纹。
