# M0–M8 Station Templates

**Status:** Proposed reusable scaffolds, not approved product specifications or implemented automation. **Authority:** [`strategy/ai-sdlc-software-factory-strategy.md`](../../strategy/ai-sdlc-software-factory-strategy.md), especially §3, §3B–§3D.

Use one template per relevant station, proportionate to the work. Populate it with real source links, stable IDs, versions, owner, and evidence. Do not create empty folders or pretend an unperformed gate passed. The station files are **human-review lenses**; their generated content must reference authoritative atomic records rather than duplicate their substance.

## Universal station-review contract

Every filled station brief must answer the following in approximately one page, linking to deeper detail when necessary:

1. **Purpose and decision:** Outcome sought, scope, current status, decision requested.
2. **Inputs:** Upstream artifact IDs, versions/hashes, governing human intent, assumptions.
3. **Changes:** Material delta from the approved baseline.
4. **Work:** 3–7 central content decisions, including alternatives if necessary.
5. **Trace/coverage:** Atomic ID links, in-scope/out-of-scope, gaps and dependencies.
6. **Verification/evidence:** Criterion/method, result and evidence reference; `NOT_EXECUTED` is not `PASSED`.
7. **Outputs/impact:** Authoritative destination, downstream consumers and invalidated evidence.
8. **Risk and convergence:** Risks, blocked causes, repair loop, attempts, cost/authority limits and restart point.
9. **Human gate:** `APPROVED`, `CONDITIONAL`, `RETURNED`, `STOPPED` or `PENDING` with owner/date and rationale.

## Station index

| Station | Template | Primary authoritative artifact(s) | Review question |
|---|---|---|---|
| M0 | [M0-explore.md](M0-explore.md) | `exploration.md` | What did we learn, and should we continue? |
| M1 | [M1-intent-ontology.md](M1-intent-ontology.md) | `product.md`, `ontology.md` | Why, for whom, and what does the domain mean? |
| M2 | [M2-business-architecture.md](M2-business-architecture.md) | `business-architecture.md` | How does the business deliver the value? |
| M3 | [M3-requirements-verification.md](M3-requirements-verification.md) | `requirements.md`, `verification-criteria.md`, FCC | What must happen, and what will prove it? |
| M4 | [M4-solution-architecture.md](M4-solution-architecture.md) | `architecture.md`, ADRs | How will the solution satisfy the constraints? |
| M5 | [M5-detailed-design.md](M5-detailed-design.md) | `design.md`, `process.md` | Is the smallest useful slice executable and testable? |
| M6 | [M6-modular-build.md](M6-modular-build.md) | `implementation.md`, code/config/build | What exact increment was built? |
| M7 | [M7-verification-evidence.md](M7-verification-evidence.md) | tests/evals/evidence and generated verification report | Does independent evidence satisfy the FCC? |
| M8 | [M8-observe-learn.md](M8-observe-learn.md) | `learning.md`, observations/deltas | Are intended outcomes achieved, and what must change? |

## Traceability and convergence rules

- Preserve `INT/OUT → TERM/ENT/REL/INV → VS/CAP/BP → REQ/AC → VG/VC/FCC → ADR/SLICE/FLOW → IMP/BUILD → TEST/EVAL/RUN/EVD → acceptance/release → OBS/RCA/DELTA` links.
- L1 repair returns to M5/M6; L2 specification or ontology gaps return to M1/M2/M3/M4; L3 outcome/intent gaps require appropriate human approval.
- Never silently weaken a requirement, AC, VC, evidence rule or ontology invariant to produce a passing result.
- A feature can be `IMPLEMENTED` without being `VERIFIED`, `ACCEPTED`, `RELEASED` or `OBSERVED`.

## Suggested review metadata

```yaml
station: M0..M8
work_id: WORK-###
feature_id: FEATURE-###
status: DRAFT
owner: TBD
source_ids: []
input_versions: []
output_ids: []
trace_ids: []
verification_ids: []
evidence_ids: []
open_gap_ids: []
human_decision: PENDING
next_action: TBD
```

Copy this contract into an actual station brief or machine-readable manifest when a real work item requires it. Do not store production execution history in the templates.
