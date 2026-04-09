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

## 2026-09-15

- Deciding body: Sample Council Meeting
- Decision: Require amendment summaries to identify the affected articles or sections, include the effective date, and be published within seven calendar days.
- Why: Amendment summaries are much more useful when readers can quickly see what changed and when the change took effect.
- Reference: `https://example.org/minutes/2026-09-15-amendment-summary-requirement`

## 2026-11-19

- Deciding body: Sample Council Meeting
- Decision: Allow emergency meetings with twenty-four hours' notice for time-sensitive business, but restrict those meetings to the urgent item named in the notice.
- Why: The council occasionally needs a faster process for narrow urgent actions, but the exception should stay limited so regular notice rules are not undermined.
- Reference: `https://example.org/minutes/2026-11-19-emergency-meeting-rule`

## 2027-02-01

- Deciding body: Sample Council Meeting
- Decision: Expand the records-retention rule to explicitly include tagged official releases and archived PDFs for at least seven years.
- Why: Continuity depends on preserving not just the current text, but also the officially adopted versions that students, advisors, and future officers may need to reference.
- Reference: `https://example.org/minutes/2027-02-01-records-retention-update`
