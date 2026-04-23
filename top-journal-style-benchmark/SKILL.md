---
name: top-journal-style-benchmark
description: Use when revising an empirical finance or economics manuscript by comparing a specific section against the closest top-journal exemplars, especially for abstracts, introductions, literature positioning, data/sample sections, empirical design, results interpretation, or conclusion. Triggers include requests to find benchmark papers, extract local PDF text, compare paragraph-by-paragraph, diagnose top-journal language gaps, revise a manuscript copy, or validate revisions with an independent reviewer/subagent.
---

# Top Journal Style Benchmark

## Overview

Use this skill to turn a local manuscript revision into a benchmarked top-journal writing pass. The workflow compares the manuscript against 1-3 close exemplar papers, diagnoses section-level language and structure gaps, revises a copy, and validates whether the revision landed.

## Core Rules

- Work from the latest source manuscript, not rendered PDF/DOCX unless no source exists.
- Never overwrite the user's current manuscript unless explicitly asked; create a clearly named revision copy.
- Prefer local PDFs, Zotero files, and project literature manifests before web search.
- Do not export or reproduce full copyrighted article text. Use local extraction for analysis, but report only short quotes, paragraph roles, and paraphrased structure.
- Match exemplars by economic object and writing job, not just keyword overlap.
- Keep empirical claims fixed unless the user explicitly asks to change results.
- Run an independent validation pass with a subagent when the user requests it or when the revision changes a high-stakes section.

## Workflow

### 1. Lock The Section And Source

Identify:

- source manuscript path;
- target section and boundaries;
- current output format needed by the user;
- whether the user allows direct edit or requires a copy;
- relevant project rules for routing drafts and outputs.

If the section is embedded in a larger draft, extract only the target section for analysis, but make revisions in a full-copy manuscript so numbering and context remain intact.

### 2. Select Benchmark Articles

Choose 1-3 benchmark articles using this hierarchy:

1. Same identification setting or institutional shock.
2. Same economic mechanism or market.
3. Same data source and empirical object.
4. Same journal style or field audience.

For each benchmark, record:

- citation, journal, and year;
- local PDF path or manifest source;
- why it is close;
- which sections are useful for comparison.

If no close local benchmark exists, search locally first with `rg`/`find`; browse only when local sources are insufficient or the user asks.

### 3. Extract Structure, Not Full Text

Use PDF/text extraction to inspect benchmark sections. Save or report:

- section headings;
- paragraph sequence and rhetorical job;
- short phrase-level examples when necessary;
- what the benchmark does not include.

Avoid copying full paragraphs from benchmark articles into new files or responses.

### 4. Compare Paragraph By Paragraph

For each manuscript paragraph or sentence group, compare:

- rhetorical job;
- claim specificity;
- mechanism continuity;
- evidence density;
- causal language;
- journal-style concision;
- whether it sounds like a result list, literature list, or process note.

Use `references/section_benchmark_rubric.md` when a detailed checklist is needed.

### 5. Revise A Copy

Create a new revision copy with a suffix that states the pass, such as:

- `P3-abstract-top-journal`
- `P4-data-benchmark`
- `P5-introduction-jf-style`

Revision principles:

- Preserve facts, coefficients, table numbers, and empirical scope.
- Replace process language with manuscript language.
- Prefer one continuous mechanism over many disconnected result claims.
- Put limitations in the right place; do not let the abstract or opening paragraph become defensive.
- If revising DOCX output too, regenerate from the revised source and verify archive validity.

### 6. Validate

Before calling the work complete:

- diff the revised section against the prior version;
- check table/figure numbering if the full manuscript was regenerated;
- search for process traces such as script, screened, filtered, audit, sample-selection, and outdated data-source names;
- verify DOCX/PDF outputs if generated;
- run a subagent review when requested.

Subagent prompt pattern:

```text
Read the revised section at <path>. Compare it against these benchmark papers and the stated revision goal. Do not edit files. Score whether the revision landed, identify inconsistencies or overclaims, and give at most 3 required fixes.
```

## Output Pattern

For a normal pass, produce:

- benchmark selection memo;
- section-by-section comparison;
- revised manuscript copy;
- optional DOCX/PDF export;
- validation notes;
- independent review summary if a subagent was used.

Keep user-facing summaries concise; link the files.
