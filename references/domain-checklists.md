# Nucl-Ex Domain Checklists

Use this reference for physics self-review, result reporting, figure QA, and referee-response preparation.

## Minimum Metadata Checklist

Every manuscript or result package should identify:

- Experiment/collaboration.
- Collision system and sqrt(s_NN).
- Run period and dataset size or integrated luminosity.
- Trigger and event selection.
- Detector subsystems.
- Centrality or event-activity estimator.
- Observable definitions.
- Kinematic ranges and acceptance.
- Correction procedure.
- Statistical and systematic uncertainties.
- Baseline or reference measurement.
- Data availability or HEPData plan.

## Observable-Specific Checks

### R_AA, R_pA, R_CP, And Ratios

- Define numerator and denominator with all normalizations.
- State pp or pA reference source and interpolation/extrapolation.
- State T_AA, N_coll, or N_part source and uncertainty.
- Separate global normalization uncertainties from point-to-point uncertainties.
- Check that ratios use compatible kinematic ranges, particle definitions, and decay corrections.

### Spectra, Yields, And Particle Ratios

- State invariant yield or cross-section convention.
- Define rapidity/pseudorapidity and pT intervals.
- State PID or signal extraction method.
- Treat feed-down, weak decays, material interactions, and branching ratios.
- Explain extrapolation to unmeasured pT if integrated yields are quoted.

### Flow v_n And Correlations

- Define method: event-plane, scalar product, cumulants, Lee-Yang zeros, template fit, or two-particle correlation.
- State eta gap and non-flow suppression.
- State centrality binning and event weights.
- Check sign conventions and harmonic definitions.
- Identify flow fluctuation sensitivity and correlation between uncertainties.

### Jets And High-pT Observables

- State jet algorithm, radius R, recombination scheme, constituent cuts, and acceptance.
- State underlying event subtraction method.
- Describe response matrix, unfolding method, regularization, and closure tests.
- Check fake-jet rejection and background fluctuation treatment.
- Identify pp reference and nuclear overlap normalization.

### Heavy Flavor, Quarkonia, And Dileptons

- State decay channels, branching ratios, signal extraction model, and mass windows.
- Separate prompt/non-prompt, feed-down, and regeneration where relevant.
- State acceptance times efficiency and polarization assumptions if applicable.
- Distinguish cold nuclear matter, recombination, screening, and energy-loss interpretations.

### Photons And Electromagnetic Probes

- State inclusive, decay, direct, or thermal photon definition.
- Explain background cocktail and subtraction.
- State isolation or conversion method when used.
- Treat material budget and conversion probability uncertainties.

### Fluctuations, Balance Functions, And Critical Observables

- Define cumulants, moments, ratios, and acceptance.
- State efficiency correction, centrality bin width correction, and volume fluctuation handling.
- Check statistical uncertainty method: bootstrap, delta theorem, subsampling, or toy MC.
- Avoid critical-point language unless baseline and noncritical effects are addressed.

### Femtoscopy And Source Imaging

- Define pair cuts, purity, Coulomb/strong FSI treatment, and fit range.
- State source parameter convention and reference frame.
- Check residual correlation and momentum-resolution corrections.

## Systematic Uncertainty Review

Create a table with:

- Source name.
- Variation or alternative method.
- Affected observable or bin range.
- Magnitude.
- Correlation type: uncorrelated, point-to-point correlated, centrality-correlated, global normalization, or shape.
- Whether it appears as boxes, bands, brackets, shaded regions, or separate table entries.

Flag problems:

- Same uncertainty counted twice.
- Global normalization uncertainty mixed with point-to-point boxes.
- Systematic variation changes physics definition rather than nuisance assumption.
- Statistical uncertainty from limited MC hidden inside a systematic source.
- Missing covariance when a fit or ratio needs correlated uncertainties.

## Figure And Table QA

Check every figure for:

- Axis labels with units.
- Collision system, sqrt(s_NN), experiment, and centrality/event class.
- Observable definition or enough caption detail to reconstruct it.
- Statistical and systematic uncertainty display.
- Model curves with version, tune, parameter set, or citation.
- Compatible y-axis normalization across panels.
- Legible marker styles in grayscale and color.
- Caption explains all symbols, bands, and boxes.

Check every HEPData table for:

- Bin edges, bin centers, and observable units.
- Statistical and systematic uncertainty columns.
- Global normalization uncertainties.
- Qualifiers: system, energy, centrality, rapidity/eta, pT, particle species, method.
- Enough metadata to reproduce the plotted points.

## Physics Claim Risk Audit

Use conservative language when:

- A model comparison is not unique.
- The effect can arise from initial-state and final-state mechanisms.
- A p-value, significance, or covariance is missing.
- The measured range does not cover the region stated in the claim.
- The baseline is interpolated, extrapolated, or from a different energy/system.
- Centrality or multiplicity selection may bias the observable.
- The conclusion depends on a single model family.

Preferred language:

- "is consistent with"
- "is described by"
- "suggests"
- "indicates within uncertainties"
- "is not sufficient to distinguish"
- "provides constraints on"

Avoid:

- "proves"
- "demonstrates conclusively"
- "model-independent evidence" unless rigorously justified.

## Reviewer Response Checklist

For each reviewer comment:

- Classify as physics, analysis method, systematic uncertainty, figure/caption, citation, wording, or formatting.
- Identify the exact manuscript location to change.
- State whether new analysis, new figure, new citation, or text-only revision is required.
- If disagreeing, give evidence and offer a clarifying edit.
- Mirror the reviewer's terminology before introducing collaboration terminology.
- Keep the reply shorter than the manuscript change unless the issue is technical.

Useful response structure:

1. Thank the reviewer for the specific point.
2. State what was changed or why no change is appropriate.
3. Quote or summarize the new manuscript text.
4. Reference figure/table/line numbers if available.
