# Student Government Governance Docs Sample

This repository is a simple example of how a student government branch could manage bylaws, constitutions, or policies with GitHub and LaTeX.

It is designed for people who may not know much about GitHub or LaTeX.

## Start Here

If you only read three things, read these:

1. This `README.md`
2. `CONTRIBUTING.md`
3. `TRANSITION.md`

## What This Repo Is Showing

This sample is meant to show:

1. what the files in a document repository look like
2. how someone makes a normal text change
3. how an approved version becomes an official release
4. how future officers can still understand the system

## The Main Idea

- `main.tex` is the source text
- `main.pdf` is the current easy-to-read PDF
- GitHub keeps the full history of changes
- GitHub Releases store official versions by date

That is the whole system.

## What Each File Does

- `main.tex`: the document text
- `main.pdf`: the current compiled PDF
- `CONTRIBUTING.md`: step-by-step instructions for making edits
- `DECISIONS.md`: a log of important repository or drafting decisions
- `TRANSITION.md`: the handoff checklist for new officers
- `.github/workflows/compile.yml`: automatically rebuilds the PDF
- `.github/workflows/release.yml`: creates an official release when run manually

## If You Have Never Used LaTeX

That is fine. Most officers should only need to do small text edits in `main.tex`.

In this repository:

- articles look like `\Article{I}{Name}`
- sections look like `\Sec{1. Example}`
- normal paragraph text is just normal text

Most people should not need to touch the formatting commands at the top of `main.tex`.

## If You Have Never Used GitHub

The important GitHub tabs are:

- `Code`: shows the files
- `Commits`: shows the history of changes
- `Actions`: shows automatic PDF builds and the manual release workflow
- `Releases`: shows official dated versions

If you are just editing text, the main thing to understand is this:

- edit the file
- save the change with a clear message
- let GitHub rebuild the PDF

## Normal Editing Workflow

For ordinary edits:

1. Edit `main.tex`.
2. Commit the change with a message that explains what changed.
3. Push to `main`.
4. GitHub Actions rebuilds `main.pdf`.
5. If needed, add a short matching note to `DECISIONS.md`.

For detailed editing instructions, see `CONTRIBUTING.md`.

## Official Release Workflow

An official release should happen only after the document change has been approved.

1. Record the approval in minutes, a vote record, or another durable source.
2. Update `main.tex` to match the approved text.
3. Add a short entry to `DECISIONS.md` if the change affects policy, structure, or workflow.
4. Push the change to `main`.
5. Run the `Release LaTeX PDF` workflow manually.
6. Fill in the required release fields.
7. GitHub creates the official release and uploads the dated PDF.

This keeps a clear separation between:

- the current working text
- the officially adopted versions

## Release Naming Scheme

This sample uses dates because dates are easier to understand than software version numbers.

- Tag: `YYYY-MM-DD`
- If there is more than one official release on the same date: `YYYY-MM-DD.1`, `YYYY-MM-DD.2`
- Release title: `Bylaws effective YYYY-MM-DD`
- PDF filename: `bylaws-YYYY-MM-DD.pdf`

Examples:

- `2026-09-15`
- `2026-11-19`
- `2027-02-01`

## Sample Release Trail In This Repo

This sample repo includes a small fake history so you can show people how diffs and releases work.

- `2026-09-15`: fuller amendment-summary requirement
- `2026-11-19`: emergency meeting notice rule
- `2027-02-01`: stronger records-retention rule

Useful demo flow:

1. Open `Releases` and click one of the dated releases.
2. Open the matching commit.
3. Use GitHub compare between two tags to show the exact changes.

Example compare ranges:

- `2026-09-15...2026-11-19`
- `2026-11-19...2027-02-01`

## What Counts As Official

- `main.tex` is the current source text
- `main.pdf` is the current convenience PDF
- Git tags and GitHub Releases are the official historical snapshots

If someone asks what the bylaws said on a certain date, look at the release or tag for that date.

## Continuity Rules

- Keep at least two people with admin access
- Keep at least two independent backups or one working mirror
- Make every official release link to its approval record
- Archive official PDFs outside GitHub as a last-resort backup

## Notes

This is a sample repository for demonstration. The proposal text itself can live in Notion. This repository shows how the system would work in practice after adoption.
