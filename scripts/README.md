# Scripts

Reusable helper scripts collected from across the zoomcamps. Each is
self-contained — copy the folder you need into a camp, or run it from here.
Python scripts use `uv` (`uv run <script>.py`).

| Script | From | What it does |
|--------|------|--------------|
| [`generate-thumbnails/`](generate-thumbnails/) | Data Engineering | Self-hosts YouTube thumbnails: downloads the raw frame, overlays a play button, commits it under `images/`, and rewrites the markdown link. Idempotent. Replaces the flaky external thumbnail service. |
| [`youtube-upload/`](youtube-upload/) | LLM | Video publishing pipeline: rename clips, clip transcripts, add chapters, and upload to YouTube from a manifest. |
| [`chop-specs/`](chop-specs/) | LLM | `chop.sh` plus per-module `.spec` files to chop long recordings into per-lesson clips. See [`../docs/video-lesson-chopping.md`](../docs/video-lesson-chopping.md). |
| [`generate-pages/`](generate-pages/) | ML, MLOps | Notebooks that generate course pages / descriptions from the module structure. |

## Conventions

- Python tooling uses `uv` with a committed `pyproject.toml` + `uv.lock`
  (see `generate-thumbnails` as the canonical example).
- Keep scripts idempotent where possible so they can be re-run safely.
- When you improve a script in one camp, update it here so the others benefit.
