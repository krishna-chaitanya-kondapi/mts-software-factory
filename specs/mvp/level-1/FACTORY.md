# Level 1 — Factory operating model
**ID:** RVC-FACTORY-MTS-L1 · **State:** To-be minimum operating model · **Status:** Draft · **Owner:** factory owner (role)

The engineering factory uses M0–M8 to build the product. The educational product uses PreRun / Run / PostRun to generate materials. Both need verifiable completion, correction and observation; their run IDs and evidence must remain distinguishable.

## K1 — Knowledge & Context Map

```mermaid
flowchart LR
  D[Domain: curriculum and sources] --> C[Resolve relevant context and versions]
  P[Product: intent quartet] --> C
  F[Factory: strategy, policies, templates] --> C
  H[History: source usage, defects, evidence] --> C
  C --> R[RunSpec / execution context]
```

| Knowledge | Authoritative location to resolve |
|---|---|
| Product and business semantics | [Intent quartet](../../../README.md#sources-and-authority) |
| Methodology | [Factory strategy](../../../strategy/ai-sdlc/ai-sdlc-software-factory-strategy.md) |
| Curriculum, content and templates | Approved run-specific Sheets/Drive references; resolve actual IDs before execution |
| Operational history | Prior release evidence and source usage; verify location and version before reuse |

Historical material is evidence, not authority. Missing required context or a conflict blocks affected work until resolved. No vector store is required initially.

## E1 — Execution Lifecycle Map

```mermaid
flowchart LR
  A[PreRun: resolve scope and preflight] --> B{Approve RunSpec}
  B -->|Authorized| C[Run: generate and independently verify]
  C --> D{Candidate DoD met?}
  D -->|Repair| C
  D -->|Yes| E[PostRun: human release gate]
  E -->|Authorized| F[Publish and reconcile]
  F --> G[Persist evidence and learn]
```

| Stage | Input → output |
|---|---|
| PreRun | Intent and context → approved revision-bound RunSpec |
| Run | Approved spec → verified candidate and QA evidence |
| PostRun | Candidate and human authority → reconciled release and closeout |

Preserve all applicable subject-specific gates (including existing Math checkpoints). A failed review returns to the affected step. See [business process rules](../../../business-architecture.md#business-rules) and [V1](DEFINITION-OF-DONE.md).

## R1 — Convergence & Recovery Map

```mermaid
flowchart TD
  A[Execute] --> B[Independent verification]
  B --> C{Applicable criteria pass?}
  C -->|Yes| D[Next authorized gate]
  C -->|No| E[Diagnose gap and impact]
  E --> F{Repair allowed and budget remains?}
  F -->|Yes| G[Targeted repair; invalidate stale checks]
  G --> B
  F -->|No| H[Block / escalate with evidence]
```

Freeze intent and criteria for the attempt. Log failed criterion IDs, evidence, correction and progress. Define retry/time budget in the approved slice contract; no numeric limit is assumed here. Stop on repeated no progress, missing authority or exhausted budget. Route semantic/intent changes to accountable owners, not silent criterion weakening. Use the strategy's distinct repair/specification/intent convergence routes.

## O1 — Observability & Learning Map

```mermaid
flowchart LR
  A[Intent and requirements] --> T[Trace IDs and versions]
  B[Engineering / generation] --> T
  C[Verification and release] --> T
  D[Runtime outcomes] --> T
  T --> L[Structured run records and evidence]
  L --> M[Metrics / gaps / defects]
  M --> N[Root cause and proposed delta]
  N --> O[Owner decision and regression]
  O -.-> A
```

Minimum events: run and correlation ID; domain/workflow or station; phase/step/attempt; actor/tool version; input/output and requirement IDs; timestamps; estimate and actual active/wait durations where measured; status; criterion results and evidence; error/correction; approval/exception; release reference. Record during execution, not reconstructed as if contemporaneous. Start with append-only structured records; dashboard later.

Review four planes from the [strategy](../../../strategy/ai-sdlc/ai-sdlc-software-factory-strategy.md#3a-intent-to-outcome-observability): intent completeness, engineering realization, verification coverage, runtime outcome. Track elapsed time, attempts, blocked steps, applicable vs executed vs passed checks, and publication reconciliation separately. Unknown measurements remain unknown.

**Open before first pilot:** exact authoritative source/config paths, slice budget, event schema and storage references, gate owners and invocation path. No executable orchestration or instrumentation is claimed by these views.

## Enforce the architecture overlays during a run

| Overlay | PreRun | Run / convergence | PostRun |
|---|---|---|---|
| Q1 | Resolve quality profile and checks | Verify, repair affected gaps, regress | Reconcile coverage and defects |
| T1 | Record actual tools, versions, access | Use approved tools; escalate unauthorized substitutions | Persist provenance |
| B1 | Approve time/retry/resource ceilings | Track known consumption; stop or escalate at limit or missing mandatory measurement | Report estimates vs actuals and cost per accepted output where measurable |
| A1 | Identify gate owners and revision | Separate producer and verifier; renew affected approvals | Human authorizes exact release; reconcile |
| S1 | Classify sources/data, credentials and destination | Treat input as untrusted, restrict access, stop on suspected security incident | Sanitize evidence and confirm permitted publication |

Baseline storage pattern from [legacy workflow mapping](https://github.com/krishna-chaitanya-kondapi/mts-crossmodel/blob/master/specs/generate_weekly_practice_worksheets/README.md): phase-first dated PreRun, Run and PostRun folders; flat approved PrintReady consumed independently by Windows printing. Validate complete in-scope batch before replacement, retain dated originals, preserve the other subject on same-week correction, serialize publishing and verify readback. Drive replacement is not atomic; finish before printing. Recovery remains a proposed control until tested live.

Minimum new telemetry: actual tool/model versions, resource usage where available, budget status, approval/invalidation events, sanitized security incidents and release recovery outcomes. Never log tokens, sensitive source content or student information. The legacy run mapping records incomplete telemetry and partial gate/publisher integration; do not report these as fully automated. See [Q1–S1](ARCHITECTURE.md#q1--quality-attribute-matrix) and [V1](DEFINITION-OF-DONE.md).
