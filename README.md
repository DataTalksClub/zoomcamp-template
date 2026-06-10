# Zoomcamp Template

The shared template and reference for DataTalks.Club Zoomcamps —
[ML](https://github.com/DataTalksClub/machine-learning-zoomcamp),
[MLOps](https://github.com/DataTalksClub/mlops-zoomcamp),
[Data Engineering](https://github.com/DataTalksClub/data-engineering-zoomcamp),
[LLM](https://github.com/DataTalksClub/llm-zoomcamp), and any new camp.

This repo exists so every zoomcamp is organized the same way and so we stop
re-inventing the same helper scripts in each one. Use it two ways:

- Starting a new zoomcamp → copy the templates and follow the checklist.
- Maintaining an existing zoomcamp → bring its READMEs and scripts in line
  with the conventions here.

## What's inside

| Path | What it is |
|------|------------|
| [`STRUCTURE.md`](STRUCTURE.md) | The canonical repo layout + README structure all camps follow |
| [`docs/conventions.md`](docs/conventions.md) | Naming, headings, banner block, and writing conventions |
| [`docs/new-zoomcamp-checklist.md`](docs/new-zoomcamp-checklist.md) | Step-by-step to spin up a new camp from these templates |
| [`templates/`](templates/) | Copy-paste README templates (root, module, cohort) + shared docs |
| [`scripts/`](scripts/) | Reusable helper scripts collected from all camps ([index](scripts/README.md)) |
| [`docs/`](docs/) | Operational guides (video pipeline, workshop best practices) |

## Quick start for a new camp

```bash
# 1. copy the templates into your new repo
cp templates/root-README.md       <new-camp>/README.md
cp templates/module-README.md     <new-camp>/01-intro/README.md
cp templates/cohort-README.md     <new-camp>/cohorts/2026/README.md
cp templates/after-sign-up.md     <new-camp>/
cp templates/learning-in-public.md <new-camp>/

# 2. fill in the {{PLACEHOLDERS}}, then follow:
#    docs/new-zoomcamp-checklist.md
```

## Why this exists

The four camps drifted apart over the years — different heading names
("How to Join" vs "How to Take" vs "How to Enroll"), emoji in some and not
others, table-of-contents in one, badges in another, and copies of the same
thumbnail/video scripts in each repo with small variations. This repo is the
single source of truth so new camps start consistent and old ones converge.

See [`STRUCTURE.md`](STRUCTURE.md) for the full spec.
