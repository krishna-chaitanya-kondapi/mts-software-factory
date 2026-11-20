# Documentation Engineering — Standard
Version: 0.1.0 · Status: proposed pilot. Governing authority and approval remain with the existing factory strategy and Reviewability Engineering.

## Table of contents
- [Principles and style](#principles-and-style)
- [Structure and depth](#structure-and-depth)
- [Examples and mental models](#examples-and-mental-models)
- [Correlation and verification](#correlation-and-verification)
- [Adoption and evolution](#adoption-and-evolution)

## Principles and style
Think from first principles, inspired by Richard Feynman: explain the problem, why the concept exists, how it works and where its boundaries lie. Use simple examples, contrast similar ideas and reconstruct the whole from its parts. Use Michael Clay Thompson-inspired precise vocabulary, clear syntax, purposeful sentences and meaningful distinctions. These are stylistic inspirations, not claims of endorsement or quotations.

Be concise without discarding requirements, decisions, qualifications, evidence or uncertainty. Prefer active, concrete language; define acronyms on first relevant use. Avoid promotional claims, repetitive prose and ornamental visuals. One authoritative home per fact. Use links instead of duplication; examples never become a new specification implicitly.

## Structure and depth
Start substantial documents with a purpose, audience, status, scope, a navigable table of contents and a substantive overview normally one to two pages. Short documents need less; Markdown page counts are approximate and depend on rendering. A concise overview should explain the whole, important relationships, decisions, constraints and gaps. Keep necessary drill-downs below or link existing authoritative sources. Avoid creating additional files merely to hide verbosity.

Use the existing [review depths and perspectives](../reviewability-engineering/REVIEWABILITY-STANDARD.md), not a competing taxonomy. L1 conceptual, L2 logical, L3 implementation and L4 technical each may have an overview and drill-down. The station artifact hierarchy in the governing strategy is a separate classification. Follow existing numbered reading order, relative navigation and canonical diagram conventions. Select structure by intent: conceptual guide emphasizes mental models; requirements emphasize obligations and acceptance; architecture emphasizes boundaries and decisions; runbook emphasizes operational steps and recovery; verification report emphasizes evidence and exceptions; ADR emphasizes alternatives and consequences.

## Examples and mental models
For easily confused terms, use a definition / distinction / concrete example table. Prefer actual workflow, artifact, contract or code references, label hypothetical examples, and never infer execution from code presence.

| Concept | Distinction | Illustrative MTS example |
|---|---|---|
| Intent | Desired outcome | A trustworthy benchmark assessment |
| Requirement | Condition the outcome must meet | A specified question count |
| Verification | Compare actual against specified criteria | Count questions in the rendered assessment |
| Evaluation | Judge quality against a rubric | Assess grade-level suitability |
| Acceptance | Authorized decision | Educator approves the exact verified revision |

Use traditional computing and human anatomy/physiology analogies when useful, not mechanically in every document. E.g. bounded feedback loops resemble iterative solvers and physiological homeostasis; neither analogy implies that the factory is literally a biological system. For protection, immunity and protective reflexes are useful analogies to distinct security controls; explain limits. Keep diagrams aligned for comparisons where possible, label arrows, use existing canonical SVGs, and follow RE visual fidelity rules.

## Correlation and verification
[RE standard](../reviewability-engineering/REVIEWABILITY-STANDARD.md) owns scope, perspective, level, review pattern, evidence, canonical fidelity, human authority and approval. DE owns explanation technique and reading structure. RE-01/05/06/07/09/10/11/12/13/14/15 cover shared concerns; do not reimplement them. The [rubric](documentation-rubric.yaml) adds eight focused checks and links shared evidence. Run applicable RE and DE checks in one report; statuses PASS, FAIL, NOT_VERIFIED, NOT_APPLICABLE with reason and evidence. An applicable blocking failure or missing evidence prevents completion. Human approval is separate from review-ready status. Use bounded correction and reverify; escalate unresolved gaps.

## Adoption and evolution
Pilot on the four Level 1 documents against their exact approved baseline. Preserve trace IDs, scope, semantics, canonical SVG bytes, original approval history and evidence limitations; new document revisions are candidates, not automatically approved. Separate material intent/architecture changes into proposed deltas. Record actual checks, limitations, revision references and human decisions. Ratify the standard and exact revised artifacts before default enforcement. Fresh-session harness discovery and runtime enforcement must be demonstrated, not assumed. Propose changes, obtain human approval, update this standard/rubric/changelog, and reuse.
