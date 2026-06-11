---
name: nucl-ex-paper-writing
description: High-energy nuclear experiment paper writing and review workflow for nucl-ex and heavy-ion manuscripts. Use when drafting, revising, HEP prose polishing, self-reviewing, citation-checking, or responding to reviewers for ALICE, STAR, PHENIX/sPHENIX, CMS-HIN, ATLAS-HI, LHC/RHIC/EIC, fixed-target, QGP, flow, spectra, jets, heavy flavor, quarkonia, correlations, femtoscopy, fluctuations, centrality, ROOT/HEPData/INSPIRE/arXiv/PDG, LaTeX, REVTeX, JHEP, NPA, PLB, PRC, PRL, or collaboration/internal review tasks.
---

# Nucl-Ex Paper Writing

## Operating Rules

Use this skill as a domain-aware writing workflow for high-energy nuclear experiment papers. Treat it as a bridge between general research-writing skills and nucl-ex-specific physics checks.

Do not invent measurements, event counts, selection cuts, systematic uncertainties, model settings, citations, or collaboration policies. If a required fact is missing, write `TODO(source needed): ...` or ask for the source.

Preserve the physical meaning of the user's draft. Improve clarity, structure, and traceability, but do not strengthen claims beyond the supplied evidence. Mark speculative interpretations as speculative.

Prefer primary sources in this order:

1. User-provided analysis notes, internal notes, tables, and approved collaboration text.
2. Published papers and official supplemental material or HEPData records.
3. INSPIRE-HEP, arXiv, DOI metadata, PDG, experiment public pages, and conference proceedings.
4. Broad discovery tools such as AMiner or Google Scholar only for leads, not final verification.

For manuscripts, use collaboration-neutral scientific tone unless the user provides a target collaboration style. Avoid "AI-humanizer" rewriting that changes technical claims, uncertainty language, or collaboration voice.

For manuscript prose, especially introductions, abstracts, captions, and interpretation paragraphs, use concrete HEP/nucl-ex prose. Do not use abstract framing, tutorial exposition, or AI-style bridge sentences as substitutes for specific physics statements.

## Quick Mode Selection

Identify the user's task and follow the matching mode.

- **Idea or paper plan**: Build a claim-evidence map, section outline, figure plan, and missing-input list.
- **Drafting from notes**: Convert notes, figures, and tables into a LaTeX-ready manuscript while preserving all caveats.
- **Results reporting**: Turn plots and fit/model comparisons into concise result paragraphs with explicit observables, systems, energies, centrality, kinematics, and uncertainties.
- **Citation verification**: Check claims against INSPIRE/arXiv/DOI/PDG/HEPData. Replace vague citations with specific references or TODOs.
- **HEP prose polish**: Rewrite drafts into natural STAR/ALICE/CMS-HIN/ATLAS-HI-style prose by removing conceptual filler and pedagogical bridge sentences while preserving technical meaning.
- **Self-review**: Audit physics consistency, figure/table readiness, uncertainty treatment, and journal/collaboration expectations.
- **Reviewer response**: Produce a response matrix, proposed manuscript edits, and polite point-by-point replies.
- **Formatting or submission**: Prepare REVTeX, JHEP/Springer, Elsevier, PRC/PRD/PRL, NPA, PLB, or collaboration-specific LaTeX outputs.

## Reference Loading

Load only the reference needed for the current task.

- Read `references/paper-structure.md` when creating an outline, drafting a paper section, reorganizing a manuscript, or adapting a generic writing skill to nucl-ex.
- Read `references/hep-prose-style.md` when drafting or polishing introductions, abstracts, result interpretations, captions, conference abstracts, or any text where the user asks for natural HEP/nucl-ex prose.
- Read `references/domain-checklists.md` when reviewing results, figures, systematics, analysis descriptions, physics claims, or self-review reports.
- Read `references/tool-adapter-map.md` when combining this skill with existing skills or tools such as claude-scholar, K-Dense scientific skills, AMiner, defuddle, ROOT MCP, INSPIRE, HEPData, docx, pdf, or pptx.

## Core Workflow

### 1. Establish Scope

Extract or ask for:

- Collision system, beam energy, experiment, run period, detector subsystems, and dataset size.
- Observable and kinematic ranges: pT, eta, rapidity, centrality, event activity, invariant mass, jet radius, species, charge, flavor, or channel.
- Analysis level: preliminary/internal, conference note, paper draft, journal submission, or response to review.
- Target venue and format: PRL, PRC, PLB, NPA, JHEP, EPJC, arXiv, or collaboration template.
- Available inputs: LaTeX draft, figures, HEPData tables, ROOT files, analysis note, systematic tables, BibTeX, referee reports.

If the target is unclear, default to a journal-neutral nucl-ex paper outline and flag venue-dependent items.

### 2. Build A Claim-Evidence Map

Before writing final prose, create a compact table with:

- Claim: the exact physics statement to appear in the paper.
- Evidence: figure/table/result supporting it.
- Scope: collision system, energy, centrality, pT/eta/y, particle species, and uncertainty.
- Baseline: pp, pA, peripheral AA, model calculation, world data, or no baseline.
- Citation: verified reference or `TODO(citation)`.
- Risk: overclaiming, missing uncertainty, unclear normalization, model dependence, or collaboration approval.

Use the claim-evidence map to decide section order and to prevent unsupported statements.

### 3. Draft Or Revise The Manuscript

Write in the usual nucl-ex order unless the target journal demands otherwise:

1. Title and abstract
2. Introduction and physics motivation
3. Experiment, dataset, and event/track/object selection
4. Corrections, backgrounds, unfolding, normalization, and systematic uncertainties
5. Results
6. Model and previous-measurement comparisons
7. Summary and outlook
8. Acknowledgments, data availability, appendices, and references

For each result paragraph, state the observable, system, energy, centrality/event class, kinematic range, uncertainty convention, and comparison baseline before interpretation.

For introductions, avoid generic QGP boilerplate. Connect the observable to a specific physics question such as collectivity, energy loss, hadronization, initial-state effects, critical behavior, equation of state, medium response, or small-system dynamics.

For prose polishing, do not rely on word-level blacklists. Keep standard HEP terms when they refer to a concrete mechanism, observable, model ingredient, or experimental consequence. Rewrite sentences whose main function is only to say that concepts are connected, viewed, framed, bridged, or understood.

For conclusions, separate:

- Direct measurement statements.
- Comparisons to prior data.
- Comparisons to models.
- Physical interpretation.
- Remaining limitations.

### 4. Verify Citations And Data Traceability

Use INSPIRE-HEP or arXiv/DOI metadata for HEP references whenever possible. Use HEPData for numerical data behind published figures when comparing results.

Check that each citation supports the statement next to it. Do not cite a review paper when a specific experimental result or model paper is needed, unless the sentence is truly a broad review statement.

For BibTeX:

- Prefer collaboration-author records from INSPIRE when available.
- Preserve arXiv identifiers.
- Include DOI when available.
- Avoid duplicate keys for the same paper.
- Mark uncertain references with `TODO(verify reference): ...`.

### 5. Audit Physics And Presentation

Before delivering a polished draft, run the relevant checks from `references/domain-checklists.md`.

Always check:

- Definitions and dimensions of observables.
- Statistical and systematic uncertainty treatment.
- Centrality, event activity, and normalization.
- Acceptance and efficiency corrections.
- Background subtraction, feed-down, pileup, fake tracks, and unfolding assumptions.
- Figure labels, units, kinematic cuts, legends, and uncertainty displays.
- Consistency between abstract, result paragraphs, captions, and conclusions.
- Whether HEPData-ready tables can reproduce the plotted points.

### 6. Produce Deliverables

Return the deliverable that matches the user's request:

- **Outline**: section tree, figure plan, missing inputs, and claim-evidence map.
- **Draft text**: LaTeX-ready sections with TODOs for missing facts.
- **Review report**: prioritized issues with file/section references, severity, and concrete fixes.
- **Reviewer response**: response table plus proposed manuscript changes.
- **Citation report**: verified, suspicious, missing, and duplicate citations.
- **Submission pass**: venue checklist, compilation notes, figure/table readiness, and unresolved blockers.

End with the highest-risk remaining TODOs rather than a generic disclaimer.
