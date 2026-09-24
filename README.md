# Eligibility Reconciliation Workbench

**Status: Concept brief.** The features below are proposed; this repository does not yet contain an implemented application or measured results.

[Portfolio](https://eskstrom.github.io/) · [Related projects](https://eskstrom.github.io/?category=healthcare-operations#library)

## Product brief

A data-quality workspace that matches synthetic member records across systems, surfaces potential duplicates, explains match confidence, and routes uncertain cases for manual review.

## Design focus

Explain record matches and preserve manual review for uncertain cases.

## Proposed scope

- Three synthetic source systems with formatting differences and duplicates.
- Deterministic and fuzzy composite matching.
- Confidence score and field-level match explanation.
- Exception queue with reviewer decision and audit log.

## Validation targets

- Precision/recall of matches against a known synthetic ground truth.
- Clear distinction between auto-match, review, and reject thresholds.

## Potential implementation

Python, DuckDB/SQLite, RapidFuzz, Streamlit.

## Guardrails

Never use real member data or real identifiers. State that the matching logic is illustrative.

[Implementation planning notes](notes/IMPLEMENTATION-NOTES.md)

<!-- portfolio-future-plans:start -->
## Future plans and PRD direction

*Planning review: 24 September 2026. These are proposed next steps, not completed work or measured outcomes.*

**Priority recommendation:** Retain in the healthcare backlog.

Build only when member-data reconciliation is the next validated problem; avoid duplicating the existing healthcare review story.

### Next scope

- [ ] Create three synthetic source systems and labeled duplicate/nonduplicate records.
- [ ] Implement an inspectable deterministic baseline before fuzzy matching.
- [ ] Define auto-match, manual-review and reject thresholds with field-level explanations and an audit trail.
- [ ] Reuse relevant data-quality checks rather than creating a separate monitoring product.

### Validation and decision criteria

Evaluate false matches, missed matches and reviewer workload against labeled ground truth. Choose thresholds explicitly and demonstrate ambiguous-case recovery. This remains a concept until implementation and validation evidence are added.
<!-- portfolio-future-plans:end -->
