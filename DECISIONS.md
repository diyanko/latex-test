# Decisions Log

This file is the permanent record of important repository and document-management decisions.

For a real branch repository, each entry should identify:

- when the decision was made
- who made it
- what was decided
- why it was decided
- where the approval record lives

The entries below are sample entries for demonstration.

## 2026-03-20

- Deciding body: Sample Student Government Working Group
- Decision: Keep each document repository flat and minimal.
- Why: New officers should be able to understand the repository in a few minutes. A flat structure reduces training burden and lowers the risk of files being misplaced.
- Reference: `https://example.org/minutes/2026-03-20-governance-repo-structure`

## 2026-03-20

- Deciding body: Sample Student Government Working Group
- Decision: Store official historical versions as Git tags and GitHub Releases rather than in `archive/` folders.
- Why: Git already preserves the full history. Releases make official versions easy to browse and download without cluttering the repository with duplicate PDFs.
- Reference: `https://example.org/minutes/2026-03-20-release-policy`

## 2026-03-27

- Deciding body: Sample Student Government Working Group
- Decision: Use date-based release tags in the format `YYYY-MM-DD`, with `.1`, `.2`, and so on only when multiple official versions occur on the same date.
- Why: Governance documents are usually looked up by effective date, not by software-style version numbers. Date-based tags are easier for future officers, advisors, and students to interpret.
- Reference: `https://example.org/minutes/2026-03-27-tagging-scheme`

## 2026-04-01

- Deciding body: Sample Student Government Working Group
- Decision: Require every official release to include a link to the approval record in the release notes.
- Why: A governing document should always be traceable back to the vote, meeting, or written approval that authorized it.
- Reference: `https://example.org/minutes/2026-04-01-approval-link-requirement`
