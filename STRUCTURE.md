# Zoomcamp Structure Spec

The canonical layout every DataTalks.Club zoomcamp should follow. Three levels
have a defined structure: the repo layout, the README at each level, and
the cohort folders.

---

## 1. Repo layout

```
<course>-zoomcamp/
├── README.md                  # course landing page (see §2)
├── 01-intro/                  # numbered module folders, NN-kebab-name
│   └── README.md              # module page (see §3)
├── 02-.../
├── ...
├── 0N-project/                # final project / capstone module
├── cohorts/
│   ├── 2024/README.md         # per-cohort schedule & deadlines (see §4)
│   ├── 2025/README.md
│   └── 2026/README.md
├── images/                    # banners, thumbnails, diagrams
├── projects/                  # (optional) project instructions + gallery
├── scripts/                   # camp-specific helper scripts
├── after-sign-up.md           # what to do after registering
├── learning-in-public.md      # learning-in-public guide
├── certificate.md             # how to get the certificate
├── awesome-<topic>.md         # (optional) curated resource list
└── .github/
    └── FUNDING.yml
```

Conventions:
- Module folders are `NN-kebab-name` (`01-intro`, `02-experiment-tracking`),
  two-digit zero-padded, so they sort correctly.
- Shared helper docs live at the repo root with the same filenames across
  all camps (`after-sign-up.md`, `learning-in-public.md`, `certificate.md`).
- Reusable cross-camp scripts live in [this template's `scripts/`](scripts/);
  copy what you need rather than re-writing.

---

## 2. Root `README.md` — canonical section order

Banner block first (image → title → tagline → signup button → link row →
badges), then these `##` sections in this order:

```
## Quick Links            — table: materials, video, Documentation, platform, Slack, Telegram, FAQ
## About the Course       — what you'll learn + duration
## Who Should Join        — target audience
## Prerequisites
## How to Take the Course — Live Cohort vs Self-Paced comparison table (see below)
## Syllabus               — one ### heading per module + bullet topics (see below)
## Projects / Capstone    — or "Final Project" (use the name that fits the course)
## Certificate            — certificate image + requirements + docs link (see below)
## Instructors
## Testimonials
## Community & Support
   ### Getting Help on Slack
   ### Learning in Public
## Sponsors
## About DataTalks.Club
```

Sections that only some courses have (FAQ, Contributing, an AI-Shipping-Labs-style
add-on) are optional; place them after Community & Support and before About
DataTalks.Club. Only include a section when there is real content for it — do not
add an empty Instructors or Testimonials section just for symmetry.

Key conventions for the variable sections:

- Quick Links: plain table, no emoji in cells. Always include a Documentation row
  linking the shared Zoomcamp Logistics docs and the course's own docs page.
- How to Take the Course: a Live Cohort vs Self-Paced comparison table (Start,
  Lectures, Homework, Leaderboard, Peer Review, Certificate, Cost, Register) plus
  a short self-paced steps list. No mermaid diagrams.
- Syllabus: one `### [Module N: Title](folder/)` heading per module, each followed
  by a bullet list of topics. No wide tables.
- Certificate: the certificate image, the requirements, and a link to the docs
  certificate/certification page.

Template: [`templates/root-README.md`](templates/root-README.md).

---

## 3. Module `NN-name/README.md` — canonical template

```
# Module N: <Title>

<1–2 sentence module overview>

## N.1 <Lesson>            — video link + short blurb
## N.2 <Lesson>
...
## Homework               — always present (link to cohort folder if external)
## Optional / Extras      — optional
## Community Notes        — standardized title
```

- Module title is `#` (h1), lessons are `##` (h2), sub-steps `###`.
- Use `N.M` numbering (e.g. `1.1`, `1.2.1`) for lessons within module N.
- Keep long install/setup instructions in a linked doc, not inline, so module
  pages stay scannable.

Template: [`templates/module-README.md`](templates/module-README.md).

---

## 4. Cohort `cohorts/<year>/README.md` — canonical template

```
# <Course> Zoomcamp <Year> Cohort

* Start date, registration link, office-hours info

## Syllabus / Schedule    — table: module | date | materials | homework
## Deadlines
## Office Hours
```

- Title is always `# <Course> Zoomcamp <Year> Cohort` (not "Edition", not bare year).

Template: [`templates/cohort-README.md`](templates/cohort-README.md).

---

## Conventions summary

See [`docs/conventions.md`](docs/conventions.md) for the full list. The headline rules:

- Banner order: image → `<h1>` title → one-line tagline → Airtable signup
  button → inline `•`-separated link row → status badges.
- No emoji in `##` headings. (Emoji are fine inside the Quick Links table.)
- Standard heading names — "How to Take the Course" (not "Join"/"Enroll"),
  "Community & Support", "About DataTalks.Club".
- Title pattern: `<Course> Zoomcamp: A Free <N>-Week Course on <topic>`.
- Let GitHub auto-generate the table of contents — don't hand-maintain one.
