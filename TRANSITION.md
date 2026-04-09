# Officer Transition Checklist

Use this checklist at every officer turnover. The goal is continuity, not ceremony.

## 1. Access

- [ ] Remove departing officers from write and admin teams.
- [ ] Add incoming officers to the correct GitHub team.
- [ ] Confirm at least two org admins remain at all times.
- [ ] Check for any direct personal collaborators who still have write access.
- [ ] Confirm the faculty advisor or designated continuity contact knows who the current admins are.

## 2. Reliability

- [ ] Run the compile workflow and confirm it succeeds.
- [ ] Confirm `main.pdf` updates correctly after a change to `main.tex`.
- [ ] Confirm the manual release workflow still appears in GitHub Actions.
- [ ] Confirm the latest release still has a downloadable PDF asset.

## 3. Governance Integrity

- [ ] Confirm officers understand that `main` holds the current official text.
- [ ] Confirm officers understand that official historical versions are stored as releases and tags.
- [ ] Confirm every official release must include an approval-record link.
- [ ] Confirm `DECISIONS.md` is being maintained for structural and workflow decisions.

## 4. Backups

- [ ] Confirm at least two independent backups or one verified mirror exist.
- [ ] Confirm at least one backup is held outside the day-to-day editing account.
- [ ] Confirm the archive location for official PDFs is still known and accessible.

## 5. Annual Review

- [ ] Verify org membership and team permissions.
- [ ] Verify automation still builds on current GitHub Actions runners.
- [ ] Verify release naming still follows the documented scheme.
- [ ] Verify the backup and archive plan is still being followed.

## Transition Rule

If incoming officers can explain the repository layout, make a text change, and publish a release by following only the files in this repository, the transition documentation is good enough.
