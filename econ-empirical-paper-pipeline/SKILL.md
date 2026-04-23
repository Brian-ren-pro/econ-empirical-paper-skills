---
name: econ-empirical-paper-pipeline
description: Use when routing a finance-oriented empirical paper workflow, choosing between writing, packaging, reviewing, and revising stages, or when the user has empirical project materials, partial drafts, complete drafts, reviewer comments, or revised manuscripts and needs the next appropriate step.
---

# Econ Empirical Paper Pipeline

## Overview

This skill is a lightweight orchestrator. It detects stage and recommends the next skill. It does not write manuscript content and does not review papers.

## Core Rules

- Do not do substantive writing; route to `econ-empirical-paper`.
- Do not do substantive review; route to `econ-empirical-paper-reviewer`.
- Do not enter full reviewer panel before a complete draft exists.
- Do not enter full evidence review without a pre-review package unless user requests prose-only review.
- Do not treat reviewer feedback as automatically correct.
- Do not auto-advance across major boundaries without user confirmation.

## Intake Questions

Determine:

- What materials exist?
- Is there a complete draft?
- Is there a pre-review package?
- Are tables/figures mapped to source files?
- Does the user want writing, review, revision, or routing?
- Are reviewer comments already available?

## Stage Routing

Read `references/stage_routing.md` for details.

Quick map:

- Idea / early materials -> `econ-empirical-paper`, architecture mode.
- Partial draft -> `econ-empirical-paper`, chapter writing or integration.
- Complete draft missing pre-review package -> `econ-empirical-paper`, pre-review packaging.
- Complete draft with pre-review package -> `econ-empirical-paper-reviewer`, full review.
- Reviewed draft -> `econ-empirical-paper`, revision mode.
- Revised draft -> optional `econ-empirical-paper-reviewer`, re-review in future versions, or ready for human review.

## Dashboard Format

Return a concise routing dashboard:

```text
Current stage: Complete Draft / Missing Explicit Pre-Review Package
Recommended next skill: econ-empirical-paper
Recommended mode: pre-review-packaging
Required materials: source draft, inline-exhibits draft, builder/exhibit map, result bundle
Exit condition: complete draft + explicit pre-review package
Next likely stage: econ-empirical-paper-reviewer
```

Then ask for confirmation before entering the recommended substantive skill.

## Handoff Requirements

Writer to reviewer:

- complete draft;
- table/figure role map;
- exhibit map;
- result summary;
- literature/mechanism summary;
- unresolved issues list.

Reviewer to writer:

- reviewer reports;
- EIC decision;
- prioritized revision roadmap;
- do-not-over-revise cautions.

