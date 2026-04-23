# Econ Empirical Paper Skills

Reusable Codex skills for empirical economics and finance paper workflows.

This repository packages four complementary skills:

- `econ-empirical-paper`: writer and revision strategist for finance-oriented empirical papers.
- `econ-empirical-paper-pipeline`: stage router that decides whether a project should move into drafting, packaging, review, or revision.
- `econ-empirical-paper-reviewer`: internal reviewer panel for full-draft critique and revision roadmaps.
- `top-journal-style-benchmark`: exemplar-based section revision against close top-journal papers.

These skills are designed for projects in areas such as corporate finance, banking, law and finance, private debt, institutional shocks, and DID-style empirical designs.

## What This Repo Is For

Use this repository when you want a reusable skill pack for paper workflows rather than a one-off prompt library.

The package is opinionated about a few things:

- lock the source package before writing;
- separate main evidence from supporting diagnostics;
- require an explicit pre-review package before full internal review;
- distinguish writing, routing, and reviewer roles;
- benchmark style against close exemplar papers instead of generic "polish" passes.

## Skill Roles

| Skill | Role | Use It When |
| --- | --- | --- |
| `econ-empirical-paper` | Writer / strategist | You need to organize materials, draft sections, integrate a full paper, or revise from reviewer comments. |
| `econ-empirical-paper-pipeline` | Stage router | You are not sure whether the project is in idea, draft, packaging, review, or revision stage. |
| `econ-empirical-paper-reviewer` | Internal reviewer panel | You already have a complete draft and want structured referee-style critique. |
| `top-journal-style-benchmark` | Style benchmarking tool | You want to revise a section by comparing it to 1 to 3 close top-journal exemplars. |

## Recommended Workflow

1. Start with `econ-empirical-paper-pipeline` if the current project stage is unclear.
2. Use `econ-empirical-paper` to build architecture, draft, integrate, and prepare the pre-review package.
3. Run `econ-empirical-paper-reviewer` only after a complete draft and explicit pre-review package exist.
4. Use `top-journal-style-benchmark` for section-level polishing once argument and evidence structure are already stable.

## Installation

Codex discovers skills from `~/.codex/skills`.

Option 1: symlink this repository's skill folders.

```bash
mkdir -p ~/.codex/skills
ln -s /path/to/econ-empirical-paper-skills/econ-empirical-paper ~/.codex/skills/econ-empirical-paper
ln -s /path/to/econ-empirical-paper-skills/econ-empirical-paper-pipeline ~/.codex/skills/econ-empirical-paper-pipeline
ln -s /path/to/econ-empirical-paper-skills/econ-empirical-paper-reviewer ~/.codex/skills/econ-empirical-paper-reviewer
ln -s /path/to/econ-empirical-paper-skills/top-journal-style-benchmark ~/.codex/skills/top-journal-style-benchmark
```

Option 2: copy the folders directly into `~/.codex/skills`.

## Example Prompts

```text
Use $econ-empirical-paper-pipeline to determine the current stage of this corporate finance paper and recommend the next workflow.
```

```text
Use $econ-empirical-paper to turn these result bundles and draft notes into a paper architecture and chapter plan.
```

```text
Use $econ-empirical-paper-reviewer to simulate an internal reviewer panel for this completed private debt paper and produce a revision roadmap.
```

```text
Use $top-journal-style-benchmark to benchmark my introduction against close JF and JFE papers, revise a copy, and validate whether the pass landed.
```

## Project-Specific Calibration

This public repository intentionally does not ship project-specific profiles, private source maps, or local absolute paths.

If you want to calibrate the skills to a specific paper project, add local reference files in your own working copy and point the relevant skill to those files. Keep those project profiles outside the public release unless you are comfortable sharing them.

## Repository Layout

```text
econ-empirical-paper-skills/
├── README.md
├── LICENSE
├── econ-empirical-paper/
├── econ-empirical-paper-pipeline/
├── econ-empirical-paper-reviewer/
└── top-journal-style-benchmark/
```

## License

This repository is released under the MIT License.
