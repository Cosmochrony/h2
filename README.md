This repository contains the source of the **H2 Cosmochrony paper**  
*Semiclassical Consistency of the Weil Representation on Heis₃(ℤ/qℤ):
Quantitative Sinc Embedding, Generator Convergence, and Aliasing Control*.

This work proves the statement formulated as **hypothesis [H2]** in version 2.0 of the Q5a paper:

> Do the rescaled Weil generators on ℓ²(ℤ/qℤ) converge, in the large-$q$ limit,
> to the position and momentum operators on $L^2(\mathbb{R})$?

The current version of Q5a does not use that framework, and this paper discharges no hypothesis of it.

## Quick Summary

- the discrete generators $\hat{X}_q$, $\hat{P}_q$ are analysed explicitly
- convergence is formulated as **strong operator convergence**
- the problem is reduced to two structural estimates:
    - a discrete Sobolev identity
    - a quantitative aliasing bound

The main result is:

> The transported operators $ι_q \hat{X}_q ι_q^*$ and $ι_q \hat{P}_q ι_q^*$
> converge strongly to $x$ and $-i\partial_x$ in $L^2(\mathbb{R})$.

## Context and Status

Q5a version 2.0 (Zenodo record 19897055) formulated a large-$q$ limit theorem (its Theorem 7.1)
under the hypotheses [H-Π1], [H-Π2], [H2], [H-w] and [H-E1], with a spectral tightness statement [C]
for its form-convergence part. [H2] is its Hypothesis 4.3.

This paper proves the statement of [H2] and nothing else in that list:

- [H-w] is open: W1 establishes no proof of it;
- the Q5a-O2 Fourier analysis rules out [H-E1] at the $q^{-1}$ scale and supersedes [C];
- the status of [H-Π1] and [H-Π2] is not examined here.

The current Q5a proves that the canonical filtration is a Fourier window on which the published
admissibility form has zero-form Mosco limit (Theorems 3.1 and 5.1), and that under its depth and
weight hypotheses no common scalar normalisation yields a toric differential limit (Theorem 6.1).
The generator convergence proved here therefore supplies no spatial limit operator.

## Core Result

> The Weil generators on $\mathrm{Heis}_3(\mathbb{Z}/q\mathbb{Z})$ converge,
> after rescaling and embedding, to the Schrödinger generators on $L^2(\mathbb{R})$.

More precisely:

- $\hat{X}_q \to x$ (multiplication operator)
- $\hat{P}_q \to -i\partial_x$ (derivative operator)
- convergence holds strongly on $\mathcal{S}(\mathbb{R})$, uniformly on bounded subsets, and extends to $L^2$

## Main Structural Results

### 1. Discrete Sobolev identity

*Result.* The finite-difference operator admits an exact decomposition:

$D_q g - g'_{\mathrm{disc}} = \frac{q}{4\pi i}(T_1 - 2I + T_{-1})g.$

Thus:

- the error is controlled purely at the ℓ² level
- no continuous structure is required at this stage
- the momentum operator is reduced to a second-order discrete term

### 2. Quantitative aliasing control

*Result.* For $\psi \in \mathcal{S}(\mathbb{R})$,

$\sum_{k\neq 0} |\hat{\psi}(\xi + kq)| \le \frac{C}{q^M}.$

Thus:

- aliasing contributions vanish uniformly
- discrete-to-continuum transfer is controlled
- all ℓ² → $L^2$ transitions are quantitative

### 3. Quasi-isometry of the sinc embedding

*Result.*

$\left|\|ι_q f\|^2_{L^2} - \|f\|^2_{\ell^2}\right| \le \frac{C}{q} N_2(\psi).$

Thus:

- the embedding is asymptotically isometric
- the estimate is reusable: an identification of an effective metric constant $A$ in terms of the
  Born–Infeld constant would use it as one ingredient, together with a supplied power-law profile
  that is not established (W1, Section 4.2)

### 4. Asymmetric convergence mechanism

*Result.*

- $X_q$: local (Taylor expansion of characters)
- $P_q$: non-local (Sobolev + aliasing)

Thus:

- the two generators require different analytical treatments
- the asymmetry is structural, not technical

### 5. Strong operator convergence

*Result.*

$ι_q \hat{X}_q ι_q^* \to x, \quad ι_q \hat{P}_q ι_q^* \to -i\partial_x.$

## Epistemic Structure of the Paper

### Input

- the Weil representation of $\mathrm{Heis}_3(\mathbb{Z}/q\mathbb{Z})$ and the sinc embedding
- the rescaled generators of Q5a version 2.0 (its Definition 4.1)

### New results

- discrete Sobolev identity (exact)
- quantitative aliasing lemma
- quasi-isometry with explicit rate
- strong convergence of the rescaled generators

### Not established here

- any hypothesis of the current Q5a
- [H-w], [H-E1], [C]
- a non-trivial limiting Dirichlet form or spatial limit operator
- the identification of a metric constant $A$

## Repository Structure

```text
paper/
├── out/      # Compiled H2 PDF
├── tex/      # LaTeX sources
└── README.md
```
# Citation

If you reference this work, please cite:

J. Beau: Semiclassical Consistency of the Weil Representation on Heis₃(ℤ/qℤ)
Zenodo, 2026.

# Acknowledgements

Portions of the structural organisation and editorial refinement
benefited from iterative interactions with large language models
used as analytical assistants.

All theoretical results and interpretations remain the sole responsibility
of the author.

# Contributions

This repository is intended as a research reference.

Feedback and further work are welcome on:

- discrete-to-continuum limits
- semiclassical analysis
- aliasing phenomena
- spectral admissibility
- effective geometry

Please open an issue to discuss technical points or extensions.
