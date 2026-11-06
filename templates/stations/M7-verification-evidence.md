# M7 — Verification & Evidence | Station Brief Template

**Work / owner / status:** `WORK-___` · TBD · DRAFT  
**Primary outputs:** Tests, evals, immutable evidence and generated verification report · `TEST-*`, `EVAL-*`, `RUN-*`, `EVD-*`, `GAP-*`, `EXC-*`

## Scope and coverage
Record product/batch/build/version, applicable REQs/ACs/VCs, explicit exclusions and unmapped criteria. No out-of-scope item counts toward the pass denominator.

## Hierarchical verification view
| CAP → REQ → AC | VG → VC | TEST/EVAL/Review → RUN | EVD | Status |
|---|---|---|---|---|
| `CAP/REQ/AC-___` | `VG/VC-___` | `TEST/RUN-___` | `EVD-___` | NOT_EXECUTED |

## Independent verification
Record test oracle, actual vs expected, validator identity/version, calibrated rubric or human adjudication, evidence hash, regressions and uncertainty. Coverage is different from execution, and execution is different from passing.

## Gap and completion decision
Link failures to `GAP/RCA` and convergence attempt history. Evaluate each `FCC-*` gate; mark `VERIFIED` only with sufficient evidence. Human risk/waiver/release decision: PENDING.
