---
name: nucl-ex-paper-writing
description: High-energy nuclear experiment writing workflow for nucl-ex/heavy-ion manuscripts, theses, captions, abstracts, citations, self-review, and referee responses. Use for ALICE, STAR, PHENIX/sPHENIX, CMS-HIN, ATLAS-HI, RHIC/LHC/EIC/fixed-target topics including QGP, spectra, flow, jets, heavy flavor, quarkonia, correlations, femtoscopy, fluctuations, centrality, HEPData, INSPIRE, arXiv, LaTeX, REVTeX, PRC/PRL/PLB/NPA/JHEP, or collaboration/internal review text.
---

# Nucl-Ex Paper Writing

## Operating Rules

Use this skill as a lightweight domain guardrail for high-energy nuclear experiment writing. Match effort to the user request; do not run a full paper-review workflow for local prose edits.

Do not invent measurements, event counts, selection cuts, systematic uncertainties, model settings, citations, or collaboration policies. If a required fact is missing, write `TODO(source needed): ...` or ask for the source.

Preserve the physical meaning of the user's draft. Improve clarity, structure, and traceability without strengthening claims beyond the supplied evidence. Mark speculative interpretations as speculative.

Prefer user-provided analysis notes, tables, approved collaboration text, published papers, official supplemental material, HEPData, INSPIRE, arXiv/DOI metadata, PDG, and experiment public pages. Use broad discovery tools only for leads.

Use collaboration-neutral scientific tone unless the user provides a target collaboration style. Write concrete HEP/nucl-ex prose, not abstract framing, tutorial exposition, or AI-style bridge sentences.

## Effort Selection

Use the smallest mode that satisfies the request.

- **Quick polish**: For sentence, paragraph, caption, abstract, or wording edits, preserve meaning and return the revised text directly. Add only brief notes for changed physics wording or missing facts.
- **Targeted section work**: For a section rewrite, result paragraph, intro, method description, or conclusion, use a compact claim-evidence check before writing only if the source text is ambiguous.
- **Deep manuscript work**: For outlines, full drafts, self-review, citation audits, submission checks, or referee responses, use the full workflow and load the relevant references.

For quick polish, do not build a claim-evidence table, ask for full metadata, browse citations, or load references unless the user asks or the text contains an unsafe physics claim.

## Reference Loading

Load only the reference needed for the current task.

- Read `references/paper-structure.md` when creating an outline, drafting a paper section, reorganizing a manuscript, or adapting a generic writing skill to nucl-ex.
- Read `references/hep-prose-style.md` when drafting or polishing introductions, abstracts, result interpretations, captions, conference abstracts, or any text where the user asks for natural HEP/nucl-ex prose.
- Read `references/domain-checklists.md` when reviewing results, figures, systematics, analysis descriptions, physics claims, or self-review reports.
- Read `references/tool-adapter-map.md` when combining this skill with existing skills or tools such as claude-scholar, K-Dense scientific skills, AMiner, defuddle, ROOT MCP, INSPIRE, HEPData, docx, pdf, or pptx.

## Core Workflow For Deep Manuscript Work

Use this workflow only for paper-scale tasks.

1. Establish scope: collision system and energy; experiment and dataset; observable and kinematics; analysis level; target venue; available draft, figures, tables, references, or referee reports.
2. Build a compact claim-evidence map when needed: claim, evidence, scope, baseline, citation, and risk.
3. Draft or revise in the standard nucl-ex order unless the venue says otherwise: abstract, introduction, experiment/dataset, analysis, results, comparisons, summary, acknowledgments/data/references.
4. For result text, state observable, system, energy, centrality/event class, kinematic range, uncertainty convention, and comparison baseline before interpretation.
5. For citation checks, prefer INSPIRE/arXiv/DOI metadata and HEPData; mark uncertain references with `TODO(verify reference): ...`.
6. For review or submission passes, use `references/domain-checklists.md` and return prioritized issues or unresolved blockers.

End with the highest-risk remaining TODOs rather than a generic disclaimer.
