---
name: econ-empirical-paper-reviewer
description: Use when a complete finance-oriented empirical paper draft needs peer-review simulation, referee reports, scoring, editorial decision, revision roadmap, methodology critique, identification critique, field positioning critique, or Devil's Advocate stress testing in corporate finance, banking, private debt, syndicated loans, law and finance, or institutional-shock designs.
---

# Econ Empirical Paper Reviewer

## Overview

This skill simulates an independent reviewer panel for finance-oriented empirical papers. It reviews; it does not rewrite. It should run after a complete draft and pre-review package exist.

## Use This For

- Full pre-submission review.
- Methodology or identification critique.
- Field-positioning critique.
- Devil's Advocate stress test.
- Revision roadmap after a complete draft.

Do not use this skill for chapter drafting. Use `econ-empirical-paper`.

## Read-Only Rule

Reviewers must not edit the manuscript. Produce reports, scores, decision letters, and revision roadmaps as separate outputs.

## Intake Gate

Before full review, check for:

- complete draft;
- table/figure role map;
- exhibit map with displayed numbering and source-file mapping;
- result-bundle summary;
- literature/mechanism summary;
- unresolved issues list.

If the exhibit map or table/figure role map is missing, pause full evidence review and ask for `econ-empirical-paper` pre-review packaging. Proceed prose-only only if the user explicitly requests it.

## Field Analysis

Create a Reviewer Configuration Card:

- primary field;
- secondary field;
- empirical design type;
- paper maturity;
- target-journal ambition if inferable;
- selected dynamic Field Reviewer profile.

Read `references/reviewer_panel_roles.md`.

## Reviewer Panel

Fixed slots:

1. Editor-in-Chief.
2. Identification Reviewer.
3. Empirical Methods Reviewer.
4. Field Reviewer.
5. Devil's Advocate.

Dynamic field profiles:

- Corporate Finance.
- Banking / Financial Intermediation.
- Law & Finance / Institutions.
- Applied Corporate Empirics.

## Literature Search Boundary

All reviewers may read supplied literature materials. Open-ended search is not default.

Bounded literature checks are allowed only for:

- Field Reviewer checking obvious missing core papers;
- EIC calibrating field or journal standards;
- explicit user request for literature completeness.

## Review Workflow

1. Intake gate.
2. Field analysis and Reviewer Configuration Card.
3. Independent reviewer reports.
4. EIC synthesis.
5. Decision and prioritized revision roadmap.

Each reviewer report must include:

- summary judgment;
- major strengths;
- major concerns;
- minor concerns;
- required revisions;
- optional revisions;
- score.

Separate concerns into:

- manuscript prose issues;
- table/result interpretation issues;
- source-material or package-completeness issues.

## Decision Scale

Use:

- `accept-like`
- `minor revision`
- `major revision`
- `reject-like`

Read `references/decision_standards.md`.

If Devil's Advocate flags a critical issue, EIC cannot issue `accept-like`.

## Scoring

Use `references/finance_review_rubric.md`. Scores are diagnostic, not real journal predictions.

## Output

Produce:

- Reviewer Configuration Card.
- Five reviewer reports.
- Score dashboard.
- EIC decision letter.
- Consensus/disagreement summary.
- Prioritized revision roadmap.
- "Do not over-revise" cautions where appropriate.

