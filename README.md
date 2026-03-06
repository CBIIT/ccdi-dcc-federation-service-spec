# CCDI DCC Federation Service Spec

This repository contains the specification and supporting documentation for the CCDI DCC Federation Service.


## Repository Structure

- `docs/` — Documentation site content and markdown pages
- `README.md` — Repository overview and quick start


## Contribution Workflow

- Sync with the latest default branch.
  - `git checkout main`
  - `git pull origin main`
- Create a branch using a clear name, for example: `docs/api-payload-example`.
  - `git checkout -b docs/api-payload-example`
- Add or update documentation in `docs/`.
- Preview and proofread content (headings, links, formatting, and examples).
- Commit with a descriptive message, for example: `docs: clarify federation response schema`.
  - `git add docs/{filename}`
  - or `git add .`
  - `git commit -m "docs: clarify federation response schema"`
- Push the branch to remote.
  - `git push -u origin docs/api-payload-example`
- Open a pull request to main branch that includes:
  - what changed
  - why the change is needed
  - any follow-up work or open questions
  - optional GitHub CLI: `gh pr create --fill`
  - add copilot as reviewer
- Address review feedback and update the same pull request until approval, merged. 



