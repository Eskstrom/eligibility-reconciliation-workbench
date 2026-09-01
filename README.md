# Eligibility Reconciliation Workbench

## Product brief

A data-quality workspace that matches synthetic member records across systems, surfaces potential duplicates, explains match confidence, and routes uncertain cases for manual review.

## Why this belongs in your portfolio

It is a direct, technically credible expression of your Firstsource reconciliation work: data lineage, exception handling, and safe automation in regulated systems.

## MVP

- Three synthetic source systems with formatting differences and duplicates.
- Deterministic and fuzzy composite matching.
- Confidence score and field-level match explanation.
- Exception queue with reviewer decision and audit log.

## Success measures

- Precision/recall of matches against a known synthetic ground truth.
- Clear distinction between auto-match, review, and reject thresholds.

## Suggested stack

Python, DuckDB/SQLite, RapidFuzz, Streamlit.

## Guardrails

Never use real member data or real identifiers. State that the matching logic is illustrative.

## Chat kickoff

“Build the Eligibility Reconciliation Workbench described here. Use synthetic data with a known ground truth and emphasize auditable exception handling.”
