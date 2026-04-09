# How To Edit This Repository

This guide is written for officers who may not know LaTeX or GitHub well.

## The Short Version

Most of the time, you only need to do one thing:

1. edit `main.tex`
2. save the change with a clear commit message
3. let GitHub rebuild the PDF

## Which File Should I Edit?

- Change the actual document text: edit `main.tex`
- Record an important workflow or drafting decision: edit `DECISIONS.md`
- Update officer handoff instructions: edit `TRANSITION.md`

Most people should not need to edit anything in `.github/workflows/`.

## Easiest Way To Make A Small Edit

If you are using GitHub in the browser:

1. Open `main.tex`
2. Click the pencil icon
3. Edit the text
4. Add a short commit message
5. Commit the change
6. Wait for GitHub Actions to rebuild `main.pdf`

Then open the updated PDF to confirm the output looks right.

## What Parts Of `main.tex` Are Safe To Edit?

Usually, edit only the body text under the title block.

Safe edits:

- changing wording in a paragraph
- adding or removing a sentence
- editing an article title
- editing a section title
- adding a new list item

Be more careful with:

- commands that start with `\`
- the formatting section near the top
- the color and layout settings

## Very Basic LaTeX Rules

You do not need to know much LaTeX to make normal edits.

- plain sentences are just typed normally
- `\Article{I}{Name}` creates an article heading
- `\Sec{1. Example}` creates a section heading
- `\textbf{word}` makes text bold
- `\&` prints `&`

If a line starts with `%`, it is a comment and does not appear in the PDF.

## Good Commit Messages

Good:

- `amend(bylaws): clarify quorum rule`
- `fix(bylaws): correct officer election wording`
- `docs: update transition checklist`

Bad:

- `update`
- `changes`
- `fix stuff`

## When To Update `DECISIONS.md`

Update `DECISIONS.md` when the group makes a decision about:

- release naming
- file structure
- drafting conventions
- archival rules
- any other change where future officers may ask "why was it done this way?"

Do not use `DECISIONS.md` for every tiny wording edit.

## How To Tell If The PDF Built Correctly

After a push:

1. open the `Actions` tab
2. open the latest `Compile LaTeX PDF` run
3. confirm it passed
4. open `main.pdf` in the repo and make sure it looks correct

## How Official Releases Work

Normal edits do not automatically become official releases.

An official release should happen only after approval.

Steps:

1. make sure the approved text is in `main.tex`
2. make sure the approval record exists
3. run the `Release LaTeX PDF` workflow
4. enter the release information
5. confirm the release page contains the approval link and PDF

## If Something Goes Wrong

If the PDF build fails:

1. open the `Actions` tab
2. read the error message
3. compare your edit to the last working commit
4. fix the text and push again

If you are unsure what broke, ask someone before changing the formatting section at the top of `main.tex`.
