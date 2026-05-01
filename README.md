This repository contains the source of the **H2 Cosmochrony paper**  
[*Semiclassical Consistency of the Weil Representation on Heis₃(ℤ/qℤ):
Quantitative Sinc Embedding, Generator Convergence, and Aliasing Control*](out/h2.pdf).

This work addresses the **[H2] hypothesis** of the Q5a programme:

> Do the rescaled Weil generators on ℓ²(ℤ/qℤ) converge, in the large-$q$ limit,
> to the position and momentum operators on $L^2(\mathbb{R})$?

## Quick Summary

H2 establishes the **operator-level consistency** of the discrete-to-continuum limit.

More precisely:

- the discrete generators $\hat{X}_q$, $\hat{P}_q$ are analysed explicitly
- convergence is formulated as **strong operator convergence**
- the problem is reduced to two structural estimates:
    - a discrete Sobolev identity
    - a quantitative aliasing bound

The main result is:

> The transported operators $ι_q \hat{X}_q ι_q^*$ and $ι_q \hat{P}_q ι_q^*$
> converge strongly to $x$ and $-i\partial_x$ in $L^2(\mathbb{R})$.

Thus H2 closes the last open hypothesis of Q5a.

## Context

**Q5a** establishes the continuum limit framework:

- fibre structure recast as Dirichlet forms
- convergence formulated as Mosco convergence
- reduction to spectral tightness

However:

- convergence of the underlying operators remained conditional
- the identification of the limit generators was not yet justified

This defines [H2].

## Core Result

The paper proves:

> The Weil generators on $\mathrm{Heis}_3(\mathbb{Z}/q\mathbb{Z})$ converge,
> after rescaling and embedding, to the Schrödinger generators on $L^2(\mathbb{R})$.

More precisely:

- $\hat{X}_q \to x$ (multiplication operator)
- $\hat{P}_q \to -i\partial_x$ (derivative operator)
- convergence holds strongly on $\mathcal{S}(\mathbb{R})$ and extends to $L^2$

## Main Structural Results

### 1. Discrete Sobolev identity

*Result.* The finite-difference operator admits an exact decomposition:

\[
D_q g - g'_{\mathrm{disc}} = \frac{q}{4\pi i}(T_1 - 2I + T_{-1})g.
\]

Thus:

- the error is controlled purely at the ℓ² level
- no continuous structure is required at this stage
- the momentum operator is reduced to a second-order discrete term

### 2. Quantitative aliasing control

*Result.* For $\psi \in \mathcal{S}(\mathbb{R})$,

\[
\sum_{k\neq 0} |\hat{\psi}(\xi + kq)| \le \frac{C}{q^M}.
\]

Thus:

- aliasing contributions vanish uniformly
- discrete-to-continuum transfer is controlled
- all ℓ² → $L^2$ transitions are quantitative

### 3. Quasi-isometry of the sinc embedding

*Result.*

$\left|\|ι_q f\|^2_{L^2} - \|f\|^2_{\ell^2}\right| \le \frac{C}{q} N_2(\psi).$

Thus:

- the embedding is asymptotically isometric
- norm defects are summable
- this estimate is reusable (Q5a-O5)

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

Thus:

- the discrete representation converges to the Schrödinger representation
- the semiclassical limit is established at operator level

## Foundational Chain from the Substrate

The derivation is fully internal:

admissibility structure  
$\to$ spectral profiles  
$\to$ tightness (Q5a)  
$\to$ valid embedding  
$\to$ operator convergence (H2)

No continuum assumption is introduced externally.

## Mathematical Role of H2

H2 provides the missing analytical closure of Q5a:

- validates the operator limit
- justifies the identification of generators
- ensures consistency of the continuum representation
- provides quantitative control of embedding

## Epistemic Structure of the Paper

### Established input

- spectral tightness framework (Q5a)
- admissible structure (O-series)
- numerical scaling behaviour (O25)

### New results

- discrete Sobolev identity (exact)
- quantitative aliasing lemma
- quasi-isometry with explicit rate
- operator convergence proof

### Closed problem

- Hypothesis [H2] is fully resolved

### Remaining open problems

- identification of the limiting Dirichlet form
- extraction of effective geometry (Q5b)
- identification of metric constant $A$ (Q5a-O5)

## Interpretation of the Result

The conceptual shift is:

- previous view: operator convergence assumed or heuristic
- H2: operator convergence is **derived and controlled**

Thus:

- the continuum limit is not only geometric
- it is also dynamically consistent
- the Schrödinger structure emerges from admissibility

## Structural Role of H2

H2 completes the Q5a programme:

- **O-series**: finite-$q$ structure
- **Q5a**: continuum reduction
- **H2**: operator convergence
- **Q5b (future)**: geometry extraction

Thus:

- existence of the limit is established
- operator structure is validated
- only geometric interpretation remains

## What H2 Adds

- exact discrete Sobolev decomposition
- quantitative aliasing control
- asymptotic quasi-isometry
- strong convergence of generators
- closure of Q5a hypothesis chain

## Outcome

The continuum limit is now:

- analytically complete
- operator-consistent
- quantitatively controlled
- structurally derived

The remaining task is no longer convergence.

It is **geometric interpretation**.

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
