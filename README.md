# Student Government Governance Docs (Test Setup)

This repository is a basic, low-maintenance test of a long-term governance workflow using GitHub + LaTeX.

## Goal

- Keep one source of truth for governing text.
- Keep a permanent, reviewable history of all edits.
- Publish official PDFs only through intentional releases.

## Repository Layout

- `main.tex`: Official source document.
- `.github/workflows/compile.yml`: Auto-compile test PDF on push/PR.
- `.github/workflows/release.yml`: Manual release only.
- `TRANSITION.md`: Officer handoff checklist.

## Day-to-Day Editing

1. Edit `main.tex`.
2. Commit with a clear message that explains why the text changed.
3. Push to `main`.
4. Confirm compile workflow passes.

## Official Release (Intentional)

Releases are manual only.

1. Open Actions -> Release LaTeX PDF.
2. Run workflow.
3. Provide:
   - `tag` (example: `v2026.04.01`)
   - `approval_record_url` (minutes, vote record, or approval issue)
4. Workflow builds PDF and publishes release with approval link in notes.

## Basic Rules

- No auto-release on push.
- Every official release must cite an approval record.
- Keep at least two people with admin access.
- Keep at least two independent backup copies (local clone and/or mirror).