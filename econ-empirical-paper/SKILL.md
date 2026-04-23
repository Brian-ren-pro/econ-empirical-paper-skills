---
name: econ-empirical-paper
description: Use when organizing, drafting, integrating, or revising finance-oriented empirical papers from existing project materials, especially corporate finance, banking, private debt, syndicated loans, law and finance, institutional shocks, DID designs, manuscript chapters, result bundles, table maps, or reviewer revision roadmaps.
---

# Econ Empirical Paper

## Overview

This skill writes and revises finance-oriented empirical papers from existing research assets. It is a writer/strategist, not a reviewer panel: its endpoint is a complete draft plus a clean pre-review package.

## Use This For

- Turning empirical project materials into a paper architecture.
- Writing or revising chapters from locked results, tables, figures, and literature notes.
- Integrating partial chapters into a complete manuscript.
- Preparing a draft for an independent reviewer panel.
- Revising a draft from a reviewer roadmap.

Do not use this skill to simulate editorial decisions or multi-reviewer reports. Use `econ-empirical-paper-reviewer` for that.

## Core Rules

- Lock the source package before writing.
- Build paper architecture before drafting.
- Separate main results from supporting diagnostics.
- Map every important claim to evidence or mark it as unresolved.
- Do not write evidence-inconsistent or unsupported claims as facts.
- Do not treat a latest convenience package as canonical unless project rules say so.
- Do not send a draft to full review without a pre-review package.

## Workflow

### Phase 0: Project Lock

Identify the current writing package and the canonical source of truth.

Create a Project Source Card covering:

- canonical source directories;
- latest writing package;
- source manuscript;
- inline-exhibits manuscript, if any;
- result bundles;
- builder scripts or exhibit maps;
- literature/mechanism notes;
- known superseded materials.

If the project contains multiple manuscript variants, apply the Manuscript Variant Rule:

- Source manuscript: prose editing and chapter structure.
- Inline-exhibits manuscript: evidence-presentation review.
- Builder script or exhibit map: table/figure numbering and source-file mapping.
- DOCX/PDF exports: rendered deliverables, not canonical source, unless the user says so.

For details, read `references/pre_review_package.md`.

### Phase 1: Paper Architecture

Before drafting, produce:

- core research question;
- shock/treatment definition;
- identification claim and limits;
- preferred interpretation;
- competing explanations;
- contribution claim;
- chapter proof order;
- table/figure role map;
- claim-evidence matrix.

Use `references/finance_empirical_architecture.md` and `references/claim_evidence_matrix.md`.

### Phase 2: Chapter Writing

Write chapter by chapter. Default finance empirical order:

1. Introduction.
2. Institutional setting, literature, and hypotheses.
3. Data, sample, variables, and empirical design.
4. Core empirical results.
5. Mechanisms, heterogeneity, extensions, and downstream outcomes.
6. Conclusion.

For each chapter, state the chapter's job, allowed claims, evidence sources, and unresolved issues.

### Phase 3: Full-Text Integration

Check the complete draft for:

- stable contribution across chapters;
- fulfilled introduction promises;
- consistent treatment definition;
- identification language that matches the design;
- correct hierarchy between main results and supporting evidence;
- coherent table/figure order;
- limitations stated without undermining the contribution.

### Phase 4: Pre-Review Packaging

Prepare a package for `econ-empirical-paper-reviewer`.

Minimum required items:

- complete draft;
- table/figure role map;
- exhibit map with display numbering and source-file mapping;
- result-bundle summary;
- literature/mechanism note summary;
- unresolved issues list.

If any item is missing, either create it or tell the user review would be prose-only.

### Revision Mode

When given reviewer feedback:

- convert comments into a revision roadmap;
- classify each item as accept, disagree, partially address, or defer;
- revise the manuscript through the same claim-evidence discipline;
- preserve a short delta log explaining what changed and why.

Reviewer comments are not automatically correct. Disagree when the evidence supports it.

## Optional Project Calibration

If the user provides a project-specific source memo, package profile, or evidence map, read it before drafting. Treat those local materials as project calibration, not as part of this reusable public skill.

## Outputs

Use concise files or sections named:

- Project Source Card
- Paper Architecture
- Claim-Evidence Matrix
- Chapter Drafts
- Full-Text Integration Notes
- Pre-Review Package
- Revision Delta Log
