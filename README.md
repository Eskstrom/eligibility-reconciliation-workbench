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
