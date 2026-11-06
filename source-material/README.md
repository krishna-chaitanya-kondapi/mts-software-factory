# Historical Source Material

Preserve earlier-stage documents here for reference and progressive consolidation. These are **non-authoritative historical inputs**; the approved product, ontology, architecture and requirements specifications elsewhere in this repository retain authority.

## Organization

```text
source-material/
└── mts/
    ├── ela/
    │   └── product/
    │       ├── product-2026-08-15.md
    │       └── product-2026-11-04.md
    ├── math/
    │   └── product/
    │       └── product-2026-10-15.md
    └── shared/
```

Dates and entries above are examples, not files that have been imported.

- Group by `<domain>/<subject>/<artifact-type>/`; create folders only when material is available.
- Default to `<artifact>-YYYY-MM-DD.<ext>`, using the **known original artifact date**, not the import date.
- If the original date is unknown, use `<artifact>-undated-01.<ext>` and record the uncertainty.
- If two versions share a date, append `-01`, `-02`, etc. Keep explicit version identifiers when those are part of the original artifact's identity.
- Use `snapshots/YYYY-MM-DD/` within a subject only when several related files form one coherent historical baseline.
- Preserve original content (including format) and source provenance. Never silently overwrite or discard historical versions.

## Lightweight inventory

Track imported items in the table below. Add rows as sources arrive; do not create placeholder artifacts.

| File | Original source / reference | Original date | Consolidation destination | Status |
|---|---|---|---|---|
| [mts/ela/product/product-2026-11-05.md](mts/ela/product/product-2026-11-05.md) | ELA worksheet-generation chat; `PRODUCT.md` v1.1 | 2026-11-05 | ELA product specification (destination pending) | pending; source baseline approved |
| [mts/ela/business-architecture/business-architecture-2026-11-05.md](mts/ela/business-architecture/business-architecture-2026-11-05.md) | ELA worksheet-generation chat; `business-architecture(1).md` v0.1 | 2026-11-05 | ELA business architecture (destination pending) | pending; source proposed |
| [mts/ela/ontology/ontology-2026-11-06.md](mts/ela/ontology/ontology-2026-11-06.md) | Repository review branch `review/ela-ontology-v1`; `ontology.md` v0.1 | 2026-11-06 | ELA ontology (destination pending) | pending; source draft for human review |

Status may be `pending`, `reviewed`, `consolidated` or `deferred`.

## Consolidation

Compare ELA, Math and other subject inputs to identify genuinely shared requirements for existing authoritative MTS specifications. Keep subject-specific distinctions in their designated specifications. Record the destination and disposition in the inventory; unresolved differences require human review. Historical files remain preserved even after consolidation.

See [the governing strategy](../strategy/ai-sdlc/ai-sdlc-software-factory-strategy.md#historical-source-material-and-consolidation).
