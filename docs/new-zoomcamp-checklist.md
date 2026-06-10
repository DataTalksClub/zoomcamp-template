# New Zoomcamp Checklist

Step-by-step to spin up a new camp from this template.

## 1. Create the repo

- [ ] Create `<course>-zoomcamp` under the DataTalksClub org.
- [ ] Add `.github/FUNDING.yml` (copy from this template).
- [ ] Add `images/` with a banner (`width="80%"`, see conventions).

## 2. Landing page

- [ ] Copy `templates/root-README.md` to `README.md`.
- [ ] Replace every `{{PLACEHOLDER}}`.
- [ ] Keep the section order from `STRUCTURE.md` §2.
- [ ] Set the title to `<Course> Zoomcamp: A Free <N>-Week Course on <topic>`.

## 3. Modules

- [ ] Create `NN-kebab-name/` folders, two-digit zero-padded.
- [ ] Copy `templates/module-README.md` into each module's `README.md`.
- [ ] Number lessons `N.M` within each module.
- [ ] Add a final project / capstone module.

## 4. Cohort

- [ ] Create `cohorts/<year>/README.md` from `templates/cohort-README.md`.
- [ ] Fill in the schedule table, deadlines, and office hours.

## 5. Shared docs

- [ ] Copy `templates/after-sign-up.md` and adapt.
- [ ] Copy `templates/learning-in-public.md` and adapt.
- [ ] Add `certificate.md`.
- [ ] Optionally add `awesome-<topic>.md`.

## 6. Tooling

- [ ] Copy `scripts/generate-thumbnails` if the camp uses self-hosted thumbnails.
- [ ] Copy `scripts/youtube-upload` + `scripts/chop-specs` if you run the video
      pipeline.
- [ ] Run scripts with `uv run`.

## 7. Final pass

- [ ] No emoji in `##`/`###` headings.
- [ ] No hand-maintained table of contents.
- [ ] Standardized heading names (see `docs/conventions.md`).
- [ ] All syllabus entries link to their module folders.
