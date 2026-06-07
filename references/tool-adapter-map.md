# Tool And Skill Adapter Map

Use this reference when combining `nucl-ex-paper-writing` with external skills, MCP servers, or document tools.

## Best-Fit External Components

### HEP And Physics Data Tools

- **INSPIRE-HEP MCP or fundamental-physics/inspire**: primary tool for HEP literature search, BibTeX, author/collaboration records, citation trails, and arXiv metadata.
- **fundamental-physics/arxiv**: use for arXiv discovery and version checks. Prefer INSPIRE for final BibTeX when available.
- **fundamental-physics/hepdata**: use for published numerical data behind HEP figures, especially spectra, cross sections, ratios, flow coefficients, limits, and model comparison tables.
- **root-mcp**: use for ROOT file inspection, TTree/branch discovery, quick histograms, invariant-mass checks, and lightweight analysis QA.
- **cerngitlab-mcp**: use for public CERN GitLab documentation, experiment frameworks, ROOT examples, and code search when relevant.
- **ParticlePhysics-MCP-Server**: use for particle properties, PDG IDs, decay modes, branching ratios, and basic particle metadata.
- **PDG**: use as authoritative reference for constants, particle properties, branching ratios, and standard definitions.

### Skills From The User's List

- **Galaxy-Dawn/claude-scholar**
  - Use `research-ideation` for paper motivation and claim framing.
  - Use `citation-verification` after adapting source hierarchy to INSPIRE/arXiv/DOI/PDG/HEPData.
  - Use `results-analysis` and `results-report` for figure-to-text conversion, but replace ML metrics with nucl-ex observables and systematics.
  - Use `paper-self-review` and `review-response` directly, with the domain checklists in this skill.
  - Use `writing-anti-ai` only for final style cleanup, never for technical reinterpretation.

- **K-Dense-AI/scientific-agent-skills**
  - Use `literature-review`, `citation-management`, `scientific-writing`, and `peer-review` after replacing PubMed-first assumptions with HEP sources.
  - Use `statistical-analysis` for fits, covariance, uncertainty propagation, significance, and ratio uncertainty checks.
  - Do not use `pubmed-database` unless the paper crosses into medical, detector materials, radiation biology, or health-physics literature.

- **canxiangcc/aminer-open-skill**
  - Use `aminer-data-search` for broad discovery, author disambiguation, and non-HEP adjacent literature.
  - Do not treat AMiner as final authority for HEP BibTeX, collaboration names, or citation counts.

- **kepano/obsidian-skills**
  - Use `defuddle` to convert web pages, documentation, conference pages, and experiment notes into clean Markdown for literature notes.

- **orchestra-research/ai-research-skills**
  - Use `ml-paper-writing` only for ML-for-HEP/ML-for-heavy-ion papers, detector reconstruction ML, unfolding ML, simulation surrogate models, or anomaly detection.
  - For ordinary nucl-ex analysis papers, use only its general figure/storyline discipline, not its NeurIPS/ICML evaluation structure.

- **veeramanikandanr48/research-paper-writer**
  - Use for a basic paper scaffold or first outline.
  - Replace generic IEEE/ACM structure with the nucl-ex structure in `paper-structure.md`.

- **skills.sh / Anthropic document skills**
  - Use `doc-coauthoring` for collaborative section-by-section drafting and reader testing.
  - Use `pdf` to extract text, tables, and figures from papers.
  - Use `docx` when working with Word drafts, comments, or tracked changes.
  - Use `pptx` for conference talks, group meeting decks, or referee-response presentation material.

- **awesome-ai-research-writing**
  - Use as a prompt library for Chinese-to-English academic editing, abstract polishing, reviewer simulation, and structure checks.
  - Verify every technical claim after stylistic rewrites.

### Tools Less Suited To Nucl-Ex

- Biomedical reporting standards such as CONSORT, STROBE, and PRISMA are usually not relevant to nucl-ex manuscripts.
- PubMed-first literature workflows are usually wrong for heavy-ion papers.
- Generic "AI detector evasion" workflows should not be used to obscure AI assistance or change scientific meaning.

## Recommended Composite Workflows

### Draft From Analysis Notes

1. Use this skill to build scope and claim-evidence map.
2. Use INSPIRE/arXiv/HEPData for references and prior measurements.
3. Use ROOT MCP only if ROOT files need inspection.
4. Draft sections with `paper-structure.md`.
5. Run self-review with `domain-checklists.md`.
6. Use docx/pdf/LaTeX tools for final file handling.

### Review An Existing Draft

1. Parse the draft and figures.
2. Build a figure-to-claim table.
3. Check citations with INSPIRE/DOI/arXiv.
4. Run the observable-specific checklist.
5. Return prioritized findings and concrete rewrite patches.

### Prepare A Reviewer Response

1. Split reviewer comments into atomic issues.
2. Classify each issue using `domain-checklists.md`.
3. Identify required manuscript edits.
4. Draft replies in a respectful point-by-point format.
5. Produce revised text snippets and a response matrix.

### Build A Literature Review

1. Start with INSPIRE query terms, arXiv categories, collaborations, observables, and collision systems.
2. Use citation snowballing from key experimental papers and reviews.
3. Pull HEPData records for numerical comparison papers.
4. Use AMiner only to broaden adjacent searches.
5. Output a claim-centered literature table, not a paper list.

## Source Hierarchy For Final Claims

Use final manuscript claims only when supported by:

1. User-supplied approved analysis material.
2. Published experiment papers and HEPData records.
3. INSPIRE/arXiv/DOI/PDG records.
4. Conference proceedings or public notes when clearly labeled.
5. Broad search engines only as discovery aids.

If the source is not strong enough, write a TODO or lower the claim strength.
