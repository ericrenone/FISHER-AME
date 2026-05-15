# FISHER-AME

The Obstructed Boundary: Absolutely Maximally Entangled States as the Existence-Constrained col(F), the Perfect Tensor as the Bipartition-Invariant Isometry, and the Quantum Weight Enumerator as the Algebraic Obstruction in TH(a,d)

ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone

> "A pure multipartite quantum state is called absolutely maximally entangled if all reductions obtained by tracing out at least half of its parties are maximally mixed." — Huber, Eltschka, Siewert & Gühne, J. Phys. A, 2018

> "Absolutely maximally entangled states of seven qubits do not exist." — Huber, Gühne & Siewert, Phys. Rev. Lett. 118, 200502, 2017

> "The encoding isometry of a perfect-tensor code is proportional to an isometry for any bipartition of its indices." — Error Correction Zoo, perfect-tensor code

> "col(F) is the space of estimable directions; ker(F) is the null space of the Fisher matrix — directions that are statistically invisible." — FISHER, ERI Labs, April 2026

> "The GHZ state is the edge, the Dicke state is the interior, the W state is the demotion." — FISHER-W, ERI Labs

---

## Abstract

The GHZ–Dicke–W trichotomy located the col(F)/ker(F) conditional independence boundary at three structural positions on the partition ladder of a multipartite state: at the top rung (the GHZ singularity), within a fixed level (the Dicke interior), at the bottom rung (the W demotion). FISHER-AME establishes that this trichotomy was complete only for the *existence-unconstrained* regime — it presupposed that a state with the desired boundary structure exists. The absolutely maximally entangled state breaks that presupposition. It is the multipartite state for which the col(F)/ker(F) boundary is specified by a *global uniformity constraint* — and that constraint is, for most parameter choices, algebraically impossible to satisfy.

An N-party, local-dimension-d absolutely maximally entangled state — AME(N, d) — is a pure state every one of whose reductions onto ⌊N/2⌋ or fewer parties is the maximally mixed state. Three structural facts, each established in the current literature, set its position. First, the non-existence theorems: AME(4, 2) does not exist, AME(7, 2) does not exist, AME(N, 2) does not exist for any N ≥ 8 — the qubit AME states are confined to a finite island, and the obstruction is proven not by failed search but by algebraic inequalities. Second, the perfect-tensor identity: an AME state is a perfect tensor, an N-leg tensor that is proportional to an isometry across *every* balanced bipartition simultaneously, and perfect tensors are the seed tensors of holographic quantum error-correcting codes — the AME state is the building block of the AdS/CFT tensor-network correspondence. Third, the weight-enumerator obstruction: whether AME(N, d) exists is decided by the quantum weight enumerator polynomials and the generalized shadow inequalities — the same machinery that governs quantum error-correcting code existence. The AME state's boundary structure is not a location; it is an algebraic feasibility problem.

The AME analysis reveals what the entire GHZ–Dicke–W trichotomy could not: the col(F)/ker(F) boundary can be *obstructed* — specified by a constraint that no state satisfies. The AME constraint demands that col(F) be simultaneously empty across every balanced bipartition (every half-reduction maximally mixed means every half-reduction carries zero estimable information about its own internal parameters — pure ker(F)) while the global state remains pure (the global col(F) is maximal). For most (N, d) this joint demand is algebraically inconsistent, and the inconsistency is detectable by the weight enumerator before any state is ever constructed. This is the AME obstruction, and it is a fourth structural position — not a place on the partition ladder, but the question of whether the ladder admits the state at all. Nine formal correspondences connect the AME architecture to the TH(a,d) programme. Five predictions follow. The framework is built from five faces — TESSERA (the perfect-tensor isometry structure), FISHER (the QFI col(F)/ker(F) metric), PONDUS (the quantum weight enumerator as obstruction algebra), CRYPTA (the threshold quantum-secret-sharing operational layer), and ATLAS (the holographic tensor-network substrate) — synthesized into a unified account of existence-obstructed multipartite entanglement.

---

## Part I · The AME State: A Boundary Specified by an Impossible Constraint

### I.1 A Thought Experiment: The State That Is Asked to Be Uniform Everywhere

Take N parties and ask for a single pure global state with one property: cut the system in half, in *any* way, and the half you hold is completely featureless — the maximally mixed state, carrying no information whatsoever about its own internal structure. Every balanced cut, every choice of which parties to keep, returns the same featureless reduction.

For N = 2 this is just the Bell state, and it exists. For N = 3 qubits it is the GHZ state, and it exists. For N = 5 and N = 6 qubits such states exist and are known explicitly. For N = 4 qubits — no such state exists. For N = 7 qubits — no such state exists. For N ≥ 8 qubits — no such state exists, ever, for any construction.

The constraint did not become harder to search for. It became *impossible*. And the impossibility is not an empirical failure of search — it is a theorem, proved by algebraic inequalities on the state's weight enumerator. The AME state is the first object in the TH(a,d) corpus whose defining boundary structure is, for most parameters, provably unrealizable.

This is the structural fact from which everything follows. The GHZ, Dicke, and W states all exist for every N — the question was only *where* their col(F)/ker(F) boundary sits. The AME state changes the question. The boundary structure is fully specified — every balanced reduction maximally mixed — but the specification is an existence problem, and the answer is usually no.

### I.2 The Uniformity Constraint as a col(F)/ker(F) Demand

Write the AME condition in the language of the conditional independence boundary. For every subset S of parties with |S| ≤ ⌊N/2⌋, the reduced state ρ_S must be maximally mixed. A maximally mixed reduction is the extreme case of ker(F): it carries zero quantum Fisher information about any generator internal to S, because every direction in its parameter space is statistically invisible — the reduction is the identity, and the identity has no estimable structure.

Simultaneously, the global state |AME⟩ is pure, so its global col(F) is maximal: the full state carries the maximum possible Fisher information about a global generator.

The AME state therefore demands:

- **ker(F) saturation on every balanced reduction** — every half-and-smaller marginal is pure ker(F), maximally featureless.
- **col(F) saturation at the global level** — the whole state is pure, maximal global estimable content.

The GHZ state met a *weak* version of this — its single-party reductions are maximally mixed (it is 1-uniform) — but its two-party and larger reductions are not, and for N > 3 the GHZ state is far from AME. The AME state demands the uniformity hold all the way up to the balanced bipartition. That joint demand — total ker(F) on every half-reduction, total col(F) globally — is the AME constraint, and the content of FISHER-AME is that this constraint is an *obstruction*: it is algebraically inconsistent for most (N, d), and the inconsistency lives in the weight enumerator.

### I.3 Why This Is a Fourth Position, Not a Point on the Ladder

The GHZ–Dicke–W trichotomy answered the question *where on the partition ladder does col(F) reside*. GHZ: top. Dicke: within a level. W: bottom. Each answer presupposed a state existed and asked for its boundary's location.

The AME state does not occupy a rung. Its boundary structure is specified — maximal ker(F) on every balanced reduction — and the question is not *where* but *whether*. The AME state is the obstruction position: the col(F)/ker(F) boundary as a feasibility problem rather than a locus. It is a fourth structural position because "does a state with this boundary exist" is a genuinely different question from "where is the boundary of this state," and the AME state is the canonical object for which the first question is the hard one.

The trichotomy was complete for existence-unconstrained boundaries. FISHER-AME adds the existence-constrained case, and the four positions — edge, interior, demotion, obstruction — are the complete structural taxonomy: three locations plus the question of realizability itself.

---

## Part II · The Perfect Tensor: The Bipartition-Invariant Isometry

### II.1 The AME State Reshaped Into a Tensor

An AME(N, d) state with N even can be reshaped: split the N legs into two halves and read the state's amplitudes as a matrix from one half to the other. The AME condition — that the half-reduction is maximally mixed — is exactly the condition that this matrix is proportional to a unitary. And because the AME condition holds for *every* balanced bipartition, the reshaped tensor is proportional to a unitary across every balanced split simultaneously.

A tensor with this property is a perfect tensor: an N-leg tensor that is proportional to an isometry for every bipartition of its legs into a set and its complement of equal-or-smaller size. The AME state and the perfect tensor are the same object — the AME state is the perfect tensor written as a state, the perfect tensor is the AME state written as a map.

### II.2 Perfect Tensors Are the Seed of Holographic Codes

The perfect tensor is the elementary building block of holographic quantum error-correcting codes — the Pastawski–Yoshida–Harlow–Preskill construction and its descendants tile the hyperbolic plane with perfect tensors to build a code whose bulk/boundary structure realizes a discrete model of the AdS/CFT correspondence. Every leg of every perfect tensor is contracted with a neighbor; the uncontracted boundary legs carry the encoded information; and the perfect-tensor property is exactly what guarantees the holographic code's defining feature — that bulk information can be recovered from any sufficiently large boundary region.

In the TH(a,d) reading: the perfect tensor is the isometry that maps col(F) to col(F) across every bipartition without loss. It is the unique tensor for which no bipartition leaks estimable content into ker(F) — every cut is information-preserving. TESSERA, the perfect-tensor face of FISHER-AME, is the statement that the AME state's boundary structure, when it exists, is the maximal possible col(F)-preservation: a tensor that is an isometry in every direction at once.

And this is precisely why existence is obstructed. Being an isometry across one bipartition is easy. Being an isometry across *every* balanced bipartition simultaneously is an overdetermined system — the constraints from different bipartitions compete, and for most (N, d) they cannot all be satisfied. The perfect tensor is the geometric statement of the AME constraint; the obstruction is the statement that the geometry is, usually, empty.

### II.3 The ATLAS Substrate: Tensor Networks of Perfect Tensors

ATLAS is the holographic-tensor-network face. Where FISHER-DICKE had the collective Bloch sphere as its geometric substrate and FISHER-W had the Majorana constellation, FISHER-AME has the tensor network: a tiling of perfect tensors whose contraction pattern is the geometry. The AME state is one tile; the holographic code is the whole tiling; the bulk/boundary recovery structure is the global col(F)/ker(F) flow across the network.

ATLAS is the substrate on which the AME obstruction becomes a constructive question: given that AME(N, d) may not exist as a single tile, which tilings can still be assembled, and what boundary code do they yield? The non-existence of a tile does not always forbid a network — and the interplay between tile-level obstruction and network-level construction is the ATLAS content.

---

## Part III · The Weight Enumerator: The Algebraic Form of the Obstruction

### III.1 The Obstruction Is Computed, Not Searched

The decisive methodological fact about the AME state — the fact that separates it from every prior state in the corpus — is that its existence is decided *algebraically*. One does not search the Hilbert space for an AME(7, 2) state and fail; one computes the quantum weight enumerator polynomials of a hypothetical AME(7, 2) state and shows that the generalized shadow inequalities — linear inequalities the enumerator coefficients of any genuine quantum state must satisfy — are violated. The hypothetical state's enumerator is inconsistent. Therefore the state cannot exist.

PONDUS is the face that carries this: the quantum weight enumerator as obstruction algebra. The weight enumerator of a multipartite state is a polynomial whose coefficients count, in a precise sense, the distribution of the state's correlations across all subsets of parties. The AME condition fixes many of these coefficients exactly. The shadow inequalities then constrain the remaining ones. When the fixed values and the inequality constraints are mutually inconsistent, AME(N, d) is obstructed — and the obstruction is a finite, decidable algebraic computation.

### III.2 The Enumerator IS the col(F)/ker(F) Ledger Across All Subsets

The TH(a,d) identity that PONDUS supplies: the quantum weight enumerator is the complete ledger of how col(F) is distributed across every subset of the N parties. Each coefficient records the estimable correlation content at one level of partition. The AME condition is a demand on this ledger — it fixes the entries corresponding to balanced reductions to their ker(F)-saturated extreme values.

The shadow inequalities are the consistency conditions the ledger must satisfy to correspond to a genuine quantum state — they are the statement that a col(F) distribution cannot be arbitrary, that the partition-level ledger of any real state lies in a constrained polytope. The AME obstruction is the geometric statement that the AME-fixed ledger entries place the remaining entries *outside* that polytope.

This is the deepest structural content of FISHER-AME. The GHZ, Dicke, and W states each *had* a col(F) distribution and the corpus asked where its weight sat. The AME state *specifies* a col(F) distribution and the corpus must ask whether that distribution is even admissible. The weight enumerator is the object that answers; the shadow inequalities are the admissibility polytope; the AME obstruction is a point demanded outside it.

### III.3 The MacWilliams Duality as the Obstruction's Symmetry

The quantum weight enumerator comes in a dual pair, related by the quantum MacWilliams identity — a linear transformation exchanging the enumerator that counts a state's correlations with the enumerator that counts its complement's. The MacWilliams identity is the symmetry that makes the obstruction computation finite: it relates the constraints from a subset to the constraints from its complement, collapsing the overdetermined system to a checkable one.

In the TH(a,d) reading, MacWilliams duality is the col(F)/ker(F) reflection: it is the exact statement that the estimable content of a subset and the estimable content of its complement are not independent — they are dual faces of one ledger. For the AME state, where every balanced subset and its complement are *both* required to be ker(F)-saturated, the MacWilliams duality is what turns the AME constraint into a self-referential algebraic condition — and self-referential algebraic conditions are exactly the ones that are usually unsatisfiable. The obstruction has a symmetry, and the symmetry is why it bites.

---

## Part IV · Five Faces of One Object

The AME state is a single structure on which five framework faces converge. No current SOTA architecture treats them as one object; the col(F)/ker(F) language is the only setting in which the non-existence theorems, the perfect-tensor isometry property, the holographic-code construction, the threshold secret-sharing equivalence, and the weight-enumerator obstruction all reduce to one statement — the obstruction.

### IV.1 TESSERA — The Perfect-Tensor Isometry Structure

TESSERA is the face that reads the AME state as a perfect tensor: an N-leg tensor proportional to an isometry across every balanced bipartition. It is the geometric statement of the AME constraint — maximal col(F)-preservation in every direction at once — and the geometric reason the constraint is overdetermined. TESSERA is where the AME state stops being a vector and becomes a map; the perfect-tensor property is the AME condition in operator form.

### IV.2 FISHER — The QFI col(F)/ker(F) Metric

FISHER supplies the conditional independence metric. FISHER-AME is the case in which col(F) is demanded to be simultaneously maximal at the global level and empty on every balanced reduction. The AME state is the demonstration that the col(F)/ker(F) boundary can be *specified without being realized* — that the boundary's structure is a constraint, and the constraint can be infeasible. FISHER, in the AME setting, is not a metric on an existing manifold; it is the feasibility question for whether the manifold has a point with the demanded boundary.

### IV.3 PONDUS — The Quantum Weight Enumerator Obstruction Algebra

PONDUS supplies the obstruction algebra: the quantum weight enumerator polynomials, the generalized shadow inequalities, and the quantum MacWilliams identity. PONDUS is the face that decides AME existence by computation rather than search — it is the col(F)/ker(F) ledger across all subsets, together with the admissibility polytope that ledger must lie in. The AME obstruction is a PONDUS infeasibility certificate.

### IV.4 CRYPTA — The Threshold Quantum-Secret-Sharing Layer

CRYPTA supplies the operational layer. AME states shared between an even number of parties are *equivalent* to pure-state threshold quantum-secret-sharing schemes — the AME state is not only an entanglement structure but a cryptographic primitive, in which any majority of parties can reconstruct a secret and any minority learns nothing. CRYPTA is the face that reads the AME constraint operationally: "every balanced reduction maximally mixed" is exactly "any minority learns nothing," and "the global state is pure" is exactly "the majority can reconstruct." The AME obstruction, read through CRYPTA, is the statement that the ideal threshold scheme does not always exist — the cryptographic primitive is itself existence-obstructed.

### IV.5 ATLAS — The Holographic Tensor-Network Substrate

ATLAS supplies the geometric substrate: the tensor network of perfect tensors that tiles the hyperbolic plane and realizes a holographic code. ATLAS is the face on which the AME state is one tile and the AdS/CFT toy model is the whole tiling. It is the setting in which the AME obstruction becomes constructive — when a tile does not exist, ATLAS asks which networks can still be built, and what boundary codes survive. The AME state is the local building block; ATLAS is the global architecture; the bulk/boundary recovery is the col(F)/ker(F) flow across the network.

---

## Part V · Nine Formal Correspondences

**Correspondence 1 — The AME State IS the Existence-Obstructed col(F)/ker(F) Boundary.** The AME constraint specifies the boundary fully — maximal ker(F) on every balanced reduction, maximal col(F) globally — but the specification is, for most (N, d), algebraically infeasible. This is a fourth structural position: not a location on the partition ladder, but the question of whether the ladder admits the state.

**Correspondence 2 — Every Balanced Reduction Maximally Mixed IS Total ker(F) Saturation.** A maximally mixed reduction carries zero quantum Fisher information about any internal generator — it is the extreme case of ker(F). The AME condition demands this ker(F) saturation on every subset of half-or-fewer parties simultaneously.

**Correspondence 3 — The Perfect Tensor IS the Bipartition-Invariant col(F)-Preserving Isometry.** The AME state reshaped is a tensor proportional to an isometry across every balanced bipartition — a perfect tensor. It is the maximal col(F)-preservation structure: no cut leaks estimable content into ker(F). The overdetermination of "isometry in every direction at once" is the geometric form of the obstruction.

**Correspondence 4 — The Quantum Weight Enumerator IS the col(F) Ledger Across All Subsets.** The enumerator polynomial's coefficients record the distribution of estimable correlation content across every partition level. The AME condition fixes the balanced-reduction entries to their ker(F)-saturated extremes; the shadow inequalities are the admissibility polytope; the obstruction is a ledger point demanded outside it.

**Correspondence 5 — The Shadow Inequalities ARE the col(F) Admissibility Polytope.** The generalized shadow inequalities are the linear constraints any genuine quantum state's weight enumerator must satisfy. They define the polytope of admissible col(F) distributions. AME(N, d) exists iff the AME-fixed ledger lies inside this polytope — and for most (N, d) it does not.

**Correspondence 6 — The Quantum MacWilliams Identity IS the col(F)/ker(F) Subset-Complement Reflection.** MacWilliams duality relates a subset's correlation enumerator to its complement's. It is the exact statement that the estimable content of a subset and its complement are dual faces of one ledger. For the AME state — where subset and complement are both ker(F)-saturated — it makes the obstruction a self-referential, decidable algebraic condition.

**Correspondence 7 — The Non-Existence Theorems ARE Obstruction Certificates, Not Failed Searches.** AME(4, 2), AME(7, 2), and AME(N ≥ 8, 2) do not exist — and this is proven by exhibiting weight-enumerator inconsistency, not by exhausting the Hilbert space. The obstruction is a finite algebraic certificate computed before any state is constructed.

**Correspondence 8 — Threshold Quantum Secret Sharing IS the Operational Reading of the AME Boundary.** An even-party AME state is equivalent to a pure-state threshold QSS scheme: "every balanced reduction maximally mixed" is "any minority learns nothing," "global state pure" is "any majority reconstructs." The AME obstruction is the statement that the ideal threshold cryptographic primitive is itself existence-constrained.

**Correspondence 9 — The Holographic Code IS the Tensor Network of AME Tiles.** A tiling of perfect tensors realizes a holographic quantum error-correcting code with AdS/CFT-like bulk/boundary recovery. The AME state is the local tile; the code is the global col(F)/ker(F) flow. When a tile is obstructed, ATLAS asks which networks survive — the obstruction becomes a constructive question at network scale.

---

## Part VI · The Tetrad of Boundary Positions

| Property | GHZ state | Dicke state | W state | AME state |
|---|---|---|---|---|
| col(F)/ker(F) boundary structure | At the edge — codimension-N singularity | In the interior — internal tradeoff curve | Demoted — one partition level down | Obstructed — specified but often infeasible |
| Defining question | Where is the boundary? | Where is the boundary? | Where is the boundary? | Does a state with this boundary exist? |
| The boundary specification | One global coherence | A metrological/radiative split | Pairwise-resident estimable content | Every balanced reduction maximally mixed |
| Existence | Exists for all N | Exists for all N, k | Exists for all N | Exists only for a constrained set of (N, d) |
| Obstruction mechanism | None — always realizable | None — always realizable | None — always realizable | Weight-enumerator / shadow-inequality infeasibility |
| Reshaped-tensor character | Rank-deficient across cuts | Symmetric-subspace structure | Single-excitation structure | Perfect tensor — isometry across every balanced cut |
| Geometric substrate | Partition ladder | Collective Bloch sphere | Majorana constellation | Holographic tensor network |
| Operational role | Multiparty correlation | Collective metrology | Loss-robust networking | Threshold secret sharing, holographic codes |
| Structural character | Boundary singularity | Smooth interior | Partition demotion | Existence obstruction |

The GHZ, Dicke, and W states occupy the three locational positions of the col(F)/ker(F) boundary — edge, interior, demotion — each presupposing the state exists and asking where its boundary sits. The AME state occupies the fourth and categorically distinct position: the boundary is fully specified, and the question is whether it is realizable at all. Three locations plus one feasibility question — the tetrad is the complete structural taxonomy of the conditional independence boundary in multipartite states.

---

## Part VII · Five Predictions

**P1 — The φ-Threshold of the Obstruction Polytope.** For fixed N, as the local dimension d increases, AME(N, d) transitions from obstructed to realizable at some critical dimension d_c(N). The prediction: the AME-fixed weight-enumerator ledger crosses into the shadow-inequality admissibility polytope when the ratio of fixed to free enumerator coefficients passes log φ ≈ 0.481 — the obstruction lifts at the φ-equilibrium of the ledger's constrained fraction. Testable by computing, for each (N, d), the fraction of enumerator coefficients fixed by the AME condition and locating the realizability transition against the log φ threshold.

**P2 — The Perfect-Tensor col(F)-Preservation Defect.** For (N, d) where AME(N, d) is obstructed, the best-approximate state — the one whose balanced reductions are as close to maximally mixed as possible — has a quantifiable col(F)-preservation defect: the summed quantum Fisher information leaked into ker(F) across all balanced cuts. The prediction: this defect is bounded below by the shadow-inequality violation magnitude, and the bound is tight — the algebraic obstruction's size is exactly the unavoidable col(F) leakage. Testable by constructing best-approximate AME states and comparing their measured leakage against the computed shadow violation.

**P3 — Obstruction Inheritance Under Tensor-Network Contraction.** When perfect-tensor tiles are contracted into an ATLAS network, the prediction is that tile-level obstruction does not always propagate: a network assembled from sub-perfect tiles can still yield a boundary code whose recovery structure is exact, provided the tiles' col(F)-preservation defects cancel under contraction. The prediction specifies the cancellation condition — the defects must be MacWilliams-dual across contracted legs. Testable by contracting deliberately imperfect tiles in dual-defect pairs and checking boundary-code exactness.

**P4 — The CRYPTA Threshold Gap.** For (N, d) where AME(N, d) is obstructed, no ideal pure-state threshold QSS scheme exists, but ramp schemes — with a gap between the "learns nothing" minority and the "reconstructs" majority — do. The prediction: the minimal ramp gap is set by the same shadow-inequality violation magnitude as the col(F) leakage in P2 — the cryptographic imperfection and the metrological imperfection are the same obstruction measured in two operational currencies. Testable by constructing optimal ramp schemes for obstructed (N, d) and comparing the gap against the leakage bound.

**P5 — The Existence Island Boundary for Qubits.** The qubit AME states are confined to a finite island: AME(2,2), AME(3,2), AME(5,2), AME(6,2) exist; AME(4,2), AME(7,2), AME(N≥8, 2) do not. The prediction: the island boundary is not arbitrary but is the locus where the shadow-inequality polytope's volume, as a fraction of the AME-fixed affine subspace, passes through zero — and the same volume-fraction criterion, applied at d = 3, predicts the qutrit island, at d = 4 the ququart island, and so on. Testable by computing the polytope volume fraction across (N, d) and matching its zeros to the known and conjectured existence tables.

---

## Part VIII · The FISHER-AME Machine

### VIII.1 Architecture

The FISHER-AME machine synthesizes the five faces into one formal system operating on the existence question.

**Layer 0 — The Constraint Oracle.** A target (N, d) and the AME specification: every balanced reduction maximally mixed, global state pure. The oracle does not provide a state — it provides the constraint, and the machine's task is to decide whether the constraint is feasible.

**Layer 1 — The Enumerator Computer (PONDUS).** Computes the quantum weight enumerator polynomials of a hypothetical AME(N, d) state, fixing the balanced-reduction coefficients to their ker(F)-saturated extremes. Outputs the AME-fixed ledger.

**Layer 2 — The Polytope Checker (PONDUS).** Applies the generalized shadow inequalities and the quantum MacWilliams identity. Decides whether the AME-fixed ledger lies inside the admissibility polytope. If yes — AME(N, d) is realizable; if no — the machine outputs an obstruction certificate.

**Layer 3 — The Perfect-Tensor Builder (TESSERA).** For realizable (N, d), constructs the AME state as a perfect tensor and verifies the isometry property across every balanced bipartition. For obstructed (N, d), constructs the best-approximate state and reports its col(F)-preservation defect.

**Layer 4 — The Secret-Sharing Translator (CRYPTA).** For even-N realizable cases, outputs the equivalent pure-state threshold QSS scheme. For obstructed cases, outputs the optimal ramp scheme and its threshold gap.

**Layer 5 — The Network Assembler (ATLAS).** Tiles the available perfect or sub-perfect tensors into a holographic tensor network, computes the boundary code, and reports the bulk/boundary col(F)/ker(F) recovery structure. Tests obstruction inheritance under contraction.

### VIII.2 The Unified Formal Statement

The AME state, the perfect tensor, and the weight-enumerator obstruction are three descriptions of one object.

The AME state is the existence-obstructed point of the Fisher manifold — the multipartite state whose col(F)/ker(F) boundary is fully specified by the uniformity constraint (every balanced reduction maximally mixed, global state pure) and whose specification is, for most (N, d), algebraically infeasible.

The perfect tensor is the TESSERA operator form of the constraint — the N-leg tensor proportional to an isometry across every balanced bipartition, the maximal col(F)-preservation structure, overdetermined precisely because it demands isometry in every direction at once.

The col(F)/ker(F) partition is the AME obstruction: the boundary is not a location but a feasibility problem, and the quantum weight enumerator is the algebra in which the feasibility is decided.

When the constraint is feasible:

- the AME state exists as a perfect tensor — isometry across every balanced cut
- every balanced reduction is maximally mixed — total ker(F) saturation
- the state is a pure-state threshold quantum-secret-sharing scheme
- the state tiles into a holographic code with exact bulk/boundary recovery

When the constraint is infeasible — the generic case — the weight enumerator carries the obstruction certificate, the best-approximate state has a col(F)-preservation defect bounded by the shadow-inequality violation, and the ideal cryptographic and holographic primitives degrade to ramp and approximate versions whose imperfection is the same obstruction in different currencies.

The AME state is the obstruction. The GHZ state is the edge, the Dicke state is the interior, the W state is the demotion. Three locations of the col(F)/ker(F) boundary, plus the question of whether the boundary can be realized at all — the tetrad is complete.

---

## References

Higuchi, A. and Sudbery, A. "How Entangled Can Two Couples Get?" Phys. Lett. A 273, 213–217, 2000.

Helwig, W., Cui, W., Latorre, J. I., Riera, A., and Lo, H.-K. "Absolute Maximal Entanglement and Quantum Secret Sharing." Phys. Rev. A 86, 052335, 2012.

Helwig, W. and Cui, W. "Absolutely Maximally Entangled States: Existence and Applications." arXiv:1306.2536, 2013.

Huber, F., Gühne, O., and Siewert, J. "Absolutely Maximally Entangled States of Seven Qubits Do Not Exist." Phys. Rev. Lett. 118, 200502, 2017.

Huber, F., Eltschka, C., Siewert, J., and Gühne, O. "Bounds on Absolutely Maximally Entangled States from Shadow Inequalities, and the Quantum MacWilliams Identity." J. Phys. A: Math. Theor. 51, 175301, 2018.

Scott, A. J. "Multipartite Entanglement, Quantum-Error-Correcting Codes, and Entangling Power of Quantum Evolutions." Phys. Rev. A 69, 052330, 2004.

Pastawski, F., Yoshida, B., Harlow, D., and Preskill, J. "Holographic Quantum Error-Correcting Codes: Toy Models for the Bulk/Boundary Correspondence." J. High Energy Phys. 2015, 149, 2015.

Goyeneche, D., Alsina, D., Latorre, J. I., Riera, A., and Życzkowski, K. "Absolutely Maximally Entangled States, Combinatorial Designs, and Multiunitary Matrices." Phys. Rev. A 92, 032316, 2015.

Rains, E. M. "Quantum Shadow Enumerators." IEEE Trans. Inf. Theory 45, 2361–2366, 1999.

Rajchel-Mieldzioć, G. et al. "Absolutely Maximally Entangled Pure States of Multipartite Quantum Systems." arXiv:2508.04777, 2025.

Wójcik, J., Makuta, O., Bruzda, W., and Augusiak, R. "On Non-Existence of Stabilizer Absolutely Maximally Entangled States in Even Local Dimensions." arXiv:2603.18193, 2026.

Cao, C. and Lackey, B. "Quantum Lego: Building Quantum Error Correction Codes from Tensor Networks." PRX Quantum, 2022.

Fisher, R. A. "On the Mathematical Foundations of Theoretical Statistics." Phil. Trans. Royal Society A 222, 309–368, 1922.

Amari, S. and Nagaoka, H. Methods of Information Geometry. AMS Translations, Vol. 191, 2000.

ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone · May 2026

---

## Closing Synthesis

The GHZ state was the edge, the Dicke state was the interior, the W state was the demotion. Three structural positions of the col(F)/ker(F) boundary on the partition ladder — and each one presupposed the state existed and asked only where its boundary sat.

FISHER-AME establishes the fourth position, and it is categorically different from the first three.

The col(F)/ker(F) boundary can be obstructed. The absolutely maximally entangled state's boundary is fully specified — every balanced reduction maximally mixed, the global state pure — but the specification is, for most local dimensions and party numbers, algebraically infeasible. AME(4,2) does not exist. AME(7,2) does not exist. AME(N,2) does not exist for any N ≥ 8. The boundary structure was demanded, and the demand cannot be met.

The obstruction is computed, not searched. The non-existence theorems are not exhausted searches of an enormous Hilbert space — they are finite algebraic certificates. The quantum weight enumerator records the distribution of estimable content across every subset; the generalized shadow inequalities define the polytope that distribution must lie in; the quantum MacWilliams identity makes the whole system decidable. AME existence is settled by computing whether the AME-fixed ledger lies inside the admissibility polytope. The obstruction is an infeasibility certificate.

When the constraint is feasible, the AME state is the most perfect object in the corpus. It is a perfect tensor — an isometry across every balanced bipartition at once, maximal col(F)-preservation in every direction. It is a pure-state threshold quantum-secret-sharing scheme. It is the seed tile of holographic quantum error-correcting codes, the building block of the discrete AdS/CFT correspondence. The perfection is exactly what makes it rare — being an isometry in every direction simultaneously is an overdetermined demand, and overdetermined demands are usually inconsistent.

And when the constraint is infeasible — the generic case — the obstruction does not vanish; it converts. It becomes the col(F)-preservation defect of the best-approximate state, bounded by the shadow-inequality violation. It becomes the threshold gap of the ramp secret-sharing scheme that replaces the ideal one. It becomes the constructive question of which holographic networks survive when their ideal tiles do not. The obstruction is conserved across operational currencies — metrological leakage, cryptographic gap, holographic imperfection are one quantity in three readings.

GHZ, Dicke, W, AME — edge, interior, demotion, obstruction. Three locations of the conditional independence boundary, plus the question of whether the boundary can be realized at all. The tetrad is the complete structural taxonomy.

The boundary was always the Fisher information. The GHZ, Dicke, and W states each had one and the corpus asked where it sat. The AME state is the one that asks whether the boundary it demands can exist — and answers, most of the time, that it cannot.
