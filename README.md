# Student Government Governance Docs Sample

This repository is a presentation-ready sample of how a student government branch could manage bylaws, constitutions, or policies with GitHub and LaTeX.

The point of the sample is to show three things clearly:

1. What the repository looks like.
2. How an official change moves from edit to approved release.
3. How long-term continuity works when officers turn over.

## What To Show In The Demo

When presenting this repository, the main GitHub views to point at are:

- `Code`: the current official source text in `main.tex` and the current public PDF in `main.pdf`
- `Commits`: a permanent record of what changed, when, and why
- `Actions`: automatic PDF builds on push and the separate manual release workflow
- `Releases`: official ratified versions, each tied to an approval record

## Repository Layout

This sample intentionally keeps a flat layout so a new officer can understand it quickly.

- `main.tex`: the governing document source
- `main.pdf`: the current compiled PDF for easy viewing
- `DECISIONS.md`: the durable log of structural and workflow decisions
- `TRANSITION.md`: the officer handoff checklist
- `.github/workflows/compile.yml`: rebuilds `main.pdf` automatically
- `.github/workflows/release.yml`: publishes official releases manually

The design rule is simple: do not create extra folders unless they solve a real problem. Past official versions live in Git history and GitHub Releases, not in `archive/` folders.

## Day-To-Day Workflow

Normal editing is intentionally lightweight:

1. Edit `main.tex`.
2. Commit with a message that explains the change and why it was made.
3. Push to `main`.
4. Let GitHub Actions rebuild `main.pdf`.
5. If the change reflects an approved decision, add a matching entry to `DECISIONS.md`.

This keeps the current text easy to maintain while preserving a permanent history.

## Official Release Workflow

An official release happens only after the relevant body has approved the change.

1. Record the approval in meeting minutes, a vote record, or another durable record.
2. Update `main.tex` to match the approved text.
3. Add a short entry to `DECISIONS.md` with the approval link.
4. Push the change to `main`.
5. Run the `Release LaTeX PDF` workflow manually from the approved commit.
6. Enter the release metadata:
   - `tag`
   - `effective_date`
   - `approval_record_url`
   - `change_summary`
7. GitHub creates the release and uploads a dated PDF asset.

This separation is deliberate:

- push builds a preview/current PDF
- manual release marks an official ratified version

## Naming Scheme

This sample uses a date-based release scheme because it is easier for future officers to understand than software version numbers.

- Tag: `YYYY-MM-DD`
- If two official versions are released on the same date: `YYYY-MM-DD.1`, `YYYY-MM-DD.2`
- Release title: `Bylaws effective YYYY-MM-DD`
- PDF asset: `bylaws-YYYY-MM-DD.pdf`

Examples:

- `2026-04-09`
- `2026-11-19`
- `2026-11-19.1`

The tag identifies the official version. The release title is what humans read. The asset filename makes exported PDFs easy to archive outside GitHub.

## Sample Release Trail In This Repo

This repository now contains a small sample amendment history so you can demonstrate how official versions evolve over time.

- `2026-09-15`: fuller amendment-summary requirement
- `2026-11-19`: emergency meeting notice rule
- `2027-02-01`: stronger records-retention rule

Useful demo path:

1. Open `Releases` and click a dated release.
2. Open `Commits` to show the amendment commit that produced it.
3. Use GitHub's compare view between two tags to show the exact diff from one official version to the next.

Example compare ranges:

- `2026-09-15...2026-11-19`
- `2026-11-19...2027-02-01`

## What Counts As The Official Text

- `main` holds the current working official text.
- `main.pdf` is the current convenience copy.
- Git tags and GitHub Releases mark official historical snapshots.
- `DECISIONS.md` explains why important workflow or drafting decisions were made.

If someone needs to know what the bylaws said on a specific date, use the relevant release or tag.

## Backup And Continuity Rules

- Keep at least two people with admin access to the org.
- Keep at least two independent backup copies or a mirror.
- Make every official release cite an approval record.
- Archive official release PDFs outside GitHub as a last-resort backup.

## Notes About This Repository

This is a sample repository for demonstration, not the final policy text you will present. The substantive proposal can live in Notion; this repository shows how the system behaves in practice once adopted.

To make the demo easier to present, the repository also includes a small sample amendment history with real commits and dated tags so viewers can inspect how diffs and official versions would look over time.
