# Level 1 — Conceptual Foundation

**Status:** Documentation Engineering v0.1 candidate pilot; revised documents await human approval. The baseline had all four Level 1 review documents individually approved. Overall Reviewability Engineering completion audit pending; implementation readiness is not established.

| Document | Review views | Existing authoritative inputs |
|---|---|---|
| [01-product.md](01-product.md) | P1 — Product Intent Canvas (approved review view) | [product](../../../product.md) |
| [02-architecture.md](02-architecture.md) | Approved review view: L1 — Business Process Landscape; I1 — Domain Concept Map; C1 — System Context; Q1 — Quality; T1 — Technology; B1 — Cost; R1 — Responsibility (legacy A1); S1 — Security | [business architecture](../../../business-architecture.md), [ontology](../../../ontology.md), [strategy](../../../strategy/ai-sdlc/ai-sdlc-software-factory-strategy.md#4-m4-the-3d-architecture-kernel) |
| [03-definition-of-done.md](03-definition-of-done.md) | V1 — Definition of Done Matrix (approved review view) | [requirement-verification mapping](../../../requirement-verification-mapping.md), [strategy verification design](../../../strategy/ai-sdlc/ai-sdlc-software-factory-strategy.md#3c-verification-driven-development-and-hierarchical-evidence) |
| [04-factory.md](04-factory.md) | Approved review view: K1 — Knowledge & Context Map; E1 — Execution Lifecycle Map; N1 — Convergence & Recovery Map (legacy R1); O1 — Observability & Learning Map | [strategy](../../../strategy/ai-sdlc/ai-sdlc-software-factory-strategy.md) |

Existing A1 (Authority) and R1 (Convergence & Recovery) are legacy MVP IDs; canonical mappings are Responsibility R1 and Convergence N1 respectively. Preserve existing IDs and use qualified namespaces in new views. See the [reviewability standard](../../../strategy/reviewability-engineering/REVIEWABILITY-STANDARD.md).

## Document reading sequence

1. [Product](01-product.md) — desired outcomes and scope.
2. [Architecture](02-architecture.md) — solution structure and constraints.
3. [Definition of Done](03-definition-of-done.md) — verification and completion contracts.
4. [Factory](04-factory.md) — knowledge, execution, convergence and learning.

The following detailed review checkpoints retain their established dependency order; they are not the document reading order.

## Minimum review sequence

1. P1: outcome, users, scope/non-scope, ownership, success criteria.
2. L1/I1/C1: core versus supporting functions, information domains, system boundaries, cross-axis alignment; all five overlays Q1/T1/B1/R1/S1; resolve material constraints and distinguish baseline from proposed controls.
3. K1: authoritative knowledge inventory, precedence, retrieval, policies, configuration, guardrail specifications and unresolved gaps.
4. E1: PreRun / Run / PostRun for educational execution, inputs/outputs, accountable human gates; distinguish software-development stations M0–M8.
5. V1: stage-specific and overall completion conditions; applicable requirement/AC/VC/FCC references, method, threshold, evidence, blocking/exception policy and owner. Distinguish verification from acceptance and publication.
6. N1: bounded correction, re-verification, progress detection, retry/time budget and escalation; preserve approvals, never change intent silently.
7. O1: structured event capture from initialization, estimate versus actual, stage timing, human wait, attempts, outcomes, evidence and defect-to-delta trace. Cover intent, engineering, verification and runtime observability proportionately.

The minimum documents may link to existing detailed artifacts instead of repeating content. A planned view is not a completed view. Review and approval are recorded explicitly. A Level 1 review does not by itself authorize implementation or release.

## First actionable slice

Use a bounded representative workflow (candidate: weekly worksheet generation), verify its inputs and existing implementation, resolve its applicable DoD, and prove generation, verification, repair and publication evidence. Selection and scope require human confirmation. Keep source management visible as a supporting function, not the central value stream.

## Supporting assets

Canonical SVGs are grouped under `diagrams/` by owning document, with original filenames and bytes preserved. They remain embedded in the documents.

[Diagram folders](diagrams/) · [MVP overview](../README.md) · [Next: Level 2](../level-2-logical-detail-and-structured-contracts/README.md)

## Documentation pilot
[Composite review report](REVIEW-REPORT.md) · [Proposed standard](../../../strategy/documentation-engineering/README.md). Read Product, Architecture, Definition of Done, Factory in the existing order. The new introductory explanation and navigation are candidates; all historical approvals apply only to the baseline.
