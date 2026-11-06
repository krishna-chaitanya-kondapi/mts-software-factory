# MTS Software Factory — Agent Operating Contract

This is the **thin, model-agnostic entry point** for ChatGPT, Codex, GitHub Copilot, Claude and other execution harnesses. It links to authoritative artifacts; it does not duplicate their full rules.

## Read in this order

1. [Canonical AI-SDLC Software Factory Strategy](strategy/ai-sdlc-software-factory-strategy.md): governing method, M0–M8, ontology, traceability, verification and autonomous convergence boundaries.
2. [Project starting instructions](strategy/project-starting-instructions.md): origin, source precedence and unresolved bootstrap questions. Interpret dated statements against current verified repository state.
3. Applicable product/domain artifacts and [station templates](templates/stations/README.md). Load only the stations and source contracts relevant to the work.
4. [Historical handoff](strategy/source-history/mts-educational-factory-conversation.md) only when current authoritative sources do not resolve an older decision. Historical narrative is not automatic approval.

## Operating rules

- **Authority:** Humans own product intent, domain semantics, material scope/risk acceptance and release. Agents may propose but must not silently rebaseline these.
- **Factory vs domain:** Factory stations, evidence formats and convergence controls are reusable across domains; MTS Math/ELA and future OMS/tax products supply domain-specific ontology, business flows and requirements.
- **Station responsibilities:** M0 exploration → M1 intent/ontology (`product.md`, `ontology.md`) → M2 business architecture (`business-architecture.md`) → M3 requirements/verification design (`requirements.md`, `verification-criteria.md`, FCC) → M4 architecture → M5 design/executable process → M6 build → M7 verification/evidence → M8 observation/learning. This is iterative, not waterfall.
- **Traceability:** Maintain stable typed IDs and links from `INT/OUT → TERM/ENT/REL/INV → VS/CAP/BP → REQ/AC → VG/VC/FCC → ADR/SLICE/FLOW → IMP/BUILD → TEST/EVAL/RUN/EVD → acceptance/release → OBS/RCA/DELTA`.
- **Verification first:** Define acceptance and verification criteria and methods before implementation when possible. Separate testing, verification, AI evals and human validation; one LLM judge's confidence is not proof.
- **Evidence before completion:** Do not equate code merged, generated outputs, test existence or passing summaries with completed features. Produce scoped, versioned evidence; distinguish `NOT_APPLICABLE`, `NOT_EXECUTED`, `BLOCKED`, `FAILED`, `PASSED`, `INCONCLUSIVE` and authorized `WAIVED`.
- **Three loops:** L1 implementation repair, L2 specification/ontology correction, L3 intent/outcome learning. Route gaps to the earliest demonstrated cause, update affected upstream truth and rerun downstream checks.
- **Bounded convergence:** Follow the FCC, explicit authority, retry/cost/time limits and no-progress stops. Checkpoint work and escalate when blocked; never weaken requirements or verification thresholds to obtain a pass.
- **Independence:** Where risk warrants, independent verification challenges the producer with source-backed checks or calibrated rubrics; retain evaluator provenance and disagreements.
- **Source integrity:** Preserve user files, existing code and worktree changes. Review before deletion, external writes, migration, large refactors or publishing.
- **One source of truth:** Station briefs are review lenses. Governed specifications, atomic entities, tests, evidence and decisions live in their designated authoritative files.

## Before claiming success

Check scope and applicability; trace every in-scope AC to VCs and executed evidence; rerun relevant regressions; explain exceptions and risks; obtain required human acceptance/release decisions. If blocked, report the gap and a resumable next action.

## Working-state declaration

Distinguish **proposed architecture**, **implemented assets**, **verified behavior**, **released versions**, and **observed outcomes**. Strategy and templates do not imply an autonomous controller is deployed.
