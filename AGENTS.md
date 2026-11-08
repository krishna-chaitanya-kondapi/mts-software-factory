# Agent entry point — MTS Software Factory

This file is a thin, model-agnostic orientation for human and AI contributors.

1. Read [project starting instructions](strategy/onboarding/project-starting-instructions.md) in full.
2. Read the governing [AI-SDLC Software Factory Strategy](strategy/ai-sdlc/ai-sdlc-software-factory-strategy.md) in full. It is currently proposed for human ratification; do not infer approval or substitute a summary.
3. Treat [historical handoff](strategy/source-history/mts-educational-factory-conversation.md) as fallback context, subordinate to approved artifacts and verified evidence.
4. Inspect the [legacy implementation](https://github.com/kpkchaitanya/mts-crossmodel) as evidence, not an automatic template.

## Operating constraints

- Preserve explicit human intent, decision ownership and review gates.
- Distinguish proposed, implemented, verified, released and accepted.
- Use atomic IDs and traceability across intent → requirement → decision → slice → test/eval → release → observation → learning → requirement delta.
- Keep governing facts in one authoritative place; use links and minimal tool-specific adapters.
- When importing or consolidating historical artifacts, follow [source-material/README.md](source-material/README.md); preserve originals and provenance, and do not treat them as authoritative.
- Do not migrate executable code or establish the permanent architecture without explicit approval.
- M0–M8 are logical stations, not a requirement for nine separate teams or agents.

## Documentation checkpoint

Before drafting or revising Markdown, apply the strategy's [documentation standard](strategy/ai-sdlc/ai-sdlc-software-factory-strategy.md#documentation-standard-for-artifact-markdown).

- Lead with a short, plain-language picture of the whole: purpose, relationships, key decisions, status and gaps. Put necessary detail below it.
- Use a visual that answers a specific question; label relationships and decisions. Avoid acronym-heavy boxes, tangled arrows and repeated flowcharts.
- Cut repeated explanations and caveats; link to the authoritative fact. Preserve IDs, policies, evidence limits and human gates.
- Before finishing, check that the overview supports routine review, the visual matches the detail, and no paragraph or table repeats another without adding needed meaning. Shorten the document in place; do not hide verbosity in extra files.

## Source provenance

This file is a new bootstrap entry point dated 2026-11-01. It does not claim to be an original strategy document or approved architecture.
