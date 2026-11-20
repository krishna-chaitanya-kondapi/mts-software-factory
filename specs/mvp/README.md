# Minimum viable factory — progressive review workspace

**Status:** draft review structure; not a replacement for the governing strategy, intent quartet or executable implementation. Scope is a lightweight starting point for the MTS educational product and its reusable factory.

## Start here

Apply the [Reviewability Engineering discipline](../../strategy/reviewability-engineering/README.md) as the complete review method; this workspace is its progressive MTS application. The standard defines classification, naming, visual fidelity and review artifact DoD.

[Level 1 — Conceptual Foundation](level-1/README.md) is the active review increment. Its fourteen views are consolidated into four short documents. Review the whole before drilling down.

| Level | Purpose | Status |
|---|---|---|
| [1](level-1/README.md) | Establish minimum viable intent, architecture and operating contracts | Draft views available |
| [2](level-2/README.md) | Resolve semantics, logical flows and structured contracts where needed | Deferred |
| [3](level-3/README.md) | Review implementation components and executable controls for selected slices | Deferred |
| [4](level-4/README.md) | Inspect technical internals and physical representations when justified | Deferred |

These are **review-depth folders**, not implementation maturity, M0–M8 stations, automation levels, or the strategy's L1/L2/L3 convergence routes. Use qualified view IDs (e.g. RVC-L3-IPS) to disambiguate. The existing strategy's station brief/spec/executable/evidence hierarchy also remains distinct.

## Authority and scope

Consult the [governing strategy](../../strategy/ai-sdlc/ai-sdlc-software-factory-strategy.md), [intent quartet](../../README.md#sources-and-authority), and [agent instructions](../../AGENTS.md). The existing quartet remains the source for product scope, business semantics and requirements/verification mappings; its draft status is preserved. MVP documents are concise review lenses with links to those sources, not parallel authorities. If a review reveals a missing or conflicting fact, record it as a proposed delta and resolve it with the owner in the authoritative artifact. Do not silently ratify, rename IDs or migrate code.

MTS review focus: Weekly Practice, Mock Assessments, Topic Mastery; Curriculum, Source and Artifact Management are supporting areas. This focus neither replaces the existing functional-area IDs nor promotes deferred diagnostics or other scope without approval. The software factory that builds software and the educational workflows that run within the product have distinct lifecycles; connect them explicitly.

## Artifact conventions

Each view uses a stable ID, scope (factory, workflow or production-run; legacy overall means factory in this workspace), state (as-is/to-be), status (draft/review/approved/superseded), owner, source references and evidence limits. Prefer one or two pages of plain-language review per document, a diagram only when it helps, and relative links. Use canonical SVG for static visual reviews; render the source before approval and commit exact approved bytes. No recreation in Mermaid unless explicitly requested. Store companions beside the review document using the standard naming convention; preserve legacy filenames and IDs. Add deeper files only to answer a concrete review question. Preserve existing atomic trace IDs.

For executable schemas, code, tests, run logs and release evidence, link to their actual authoritative locations rather than copying them here. No production credentials, student records or private source materials in this public repository.

## Cross-cutting overlays

Q1 quality, T1 technology, B1 cost, A1 authority (canonical Responsibility R1) and S1 security are Level 1 architecture views, progressively elaborated only where a slice needs them. Keep the four-document model; link constraints to execution, bounded recovery, evidence and DoD. See [architecture](level-1/ARCHITECTURE.md#q1--quality-attribute-matrix).

## Incremental exit rule

Review the minimum foundation, select a bounded vertical slice, establish its applicable completion contract, execute it, record evidence, demonstrate bounded repair and review the outcome. Expand documentation only when a gap prevents safe execution or review. Do not wait for every deeper view to be produced.
