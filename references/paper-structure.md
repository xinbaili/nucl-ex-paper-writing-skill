# Nucl-Ex Paper Structure

Use this reference when outlining, drafting, or reorganizing high-energy nuclear experiment manuscripts.

## Standard Section Logic

### Abstract

Include only what can be supported by the final figures and tables:

- Observable and particle/object species.
- Collision system and sqrt(s_NN).
- Experiment and dataset if relevant.
- Centrality or event activity classes.
- Kinematic range.
- Main qualitative result.
- Most important comparison or physics implication.

Avoid detector, trigger, or method detail unless it is central to the novelty.

### Introduction

Use a narrow motivation chain:

1. Physics problem: QGP property, energy loss, hadronization, collectivity, initial state, criticality, chiral effects, baryon stopping, or medium response.
2. Observable sensitivity: explain what the measured observable constrains.
3. Prior measurements: identify the most relevant measurements and remaining gap.
4. This paper: state what is newly measured and why the dataset or method matters.

Do not use a generic "heavy-ion collisions create QGP" paragraph unless the paper is aimed at a broad journal.

### Experiment And Dataset

Report:

- Experiment and detector subsystems used.
- Collision system, sqrt(s_NN), run period, integrated luminosity or event count.
- Trigger and event selection.
- Vertex and pileup rejection.
- Centrality or multiplicity estimator and calibration source.
- Track, cluster, jet, muon, electron, photon, PID, or object selection.
- Simulation setup used for corrections, if any.

### Analysis Method

Include enough detail to reproduce the analysis logic:

- Signal extraction or object reconstruction.
- Background estimation and subtraction.
- Efficiency, acceptance, and resolution corrections.
- Unfolding or bin migration treatment.
- Feed-down or contamination corrections.
- Normalization and event weighting.
- Statistical method, fit model, covariance, or hypothesis test.

For derived observables, define every symbol near first use.

### Systematic Uncertainties

Separate uncertainty sources by origin:

- Event and centrality selection.
- Tracking, reconstruction, PID, trigger, and matching.
- Signal extraction or background model.
- Correction factors and MC modeling.
- Unfolding regularization or response matrix.
- Normalization, luminosity, T_AA, N_coll, or branching ratios.
- Model-dependent extrapolation or reference interpolation.

State which uncertainties are point-to-point correlated, global normalization, centrality-correlated, or uncorrelated when this affects interpretation.

### Results

For each figure:

1. Introduce what is plotted.
2. State the system, energy, centrality/event class, and kinematic interval.
3. Describe the visible trend.
4. Quantify only when numbers are supplied.
5. Compare to baselines or models.
6. Interpret cautiously, tied to the observable sensitivity.

Avoid repeating caption text unless it helps the physics argument.

### Model Comparisons

Identify model class and physics content:

- Hydrodynamics: initial condition, eta/s, bulk viscosity, afterburner.
- Transport: partonic/hadronic stages, cross sections, mean fields, coalescence.
- Energy-loss: radiative/collisional, path-length dependence, medium profile.
- Statistical/thermal: chemical freeze-out, canonical effects, resonance feed-down.
- pQCD/nPDF/CGC: initial-state modifications and factorization assumptions.

Do not call model-data agreement "proof"; say "consistent with", "described by", "underpredicted", or "overpredicted" within the stated uncertainties.

### Summary

Use four compact moves:

1. What was measured.
2. The strongest experimental trend.
3. What the comparison to prior data or models implies.
4. What remains open.

Do not introduce new references, new caveats, or new claims in the summary unless they were already established.

## Figure Plan Patterns

- Figure 1: Analysis overview, signal extraction example, or key corrected spectra.
- Figure 2: Main observable versus pT, centrality, rapidity, mass, or event activity.
- Figure 3: Nuclear modification, ratio, or comparison to baseline.
- Figure 4: Model comparisons.
- Figure 5: Summary trend versus centrality, N_part, multiplicity, sqrt(s_NN), or system size.

For short papers, compress method validation into supplemental material or appendices if allowed.

## Common Nucl-Ex Paper Types

### Spectra And Yields

Emphasize correction chain, normalization, PID/signal extraction, feed-down, extrapolation, and integrated yield extraction.

### Flow And Correlations

Emphasize method definition, eta gaps, non-flow suppression, event-plane or cumulant method, flow fluctuations, centrality bias, and covariance.

### Jet And High-pT

Emphasize background density, unfolding, jet radius, constituent cuts, fake jets, pp reference, R_AA/R_CP definitions, and energy-loss interpretation.

### Heavy Flavor And Quarkonia

Emphasize decay channel, signal extraction, prompt/non-prompt separation, acceptance times efficiency, feed-down, branching ratios, rapidity and pT coverage, and CNM/QGP separation.

### Femtoscopy And Correlations

Emphasize pair selection, Coulomb/strong final-state interactions, source function or fit assumptions, residual correlations, and purity corrections.

### Fluctuations And Criticality

Emphasize centrality bin width correction, efficiency correction, volume fluctuations, cumulant definitions, acceptance, and statistical uncertainty estimation.
