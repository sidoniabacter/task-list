# Workflow

How a change gets from an idea to the main branch. Read this before opening a
pull request or making a release.

## For each task

1. Write or update the spec in docs/specs/, starting from docs/specs/TEMPLATE.md.
2. Ask the agent for a plan first, then for the code.
3. Read the diff, run the project, run bin/check.
4. Write what happened in docs/ai-log.md.
5. Commit, push, open a pull request.

## Pull requests

- Title: short and descriptive (e.g., "Add login page with Tailwind")
- Description: link to the spec, screenshots if UI changes
- At least one approval required before merging
- All checks must pass (bin/check, future CI)

## Commits

- Follow conventions from docs/conventions.md
- Squash related commits before creating a PR
- Rebase onto main before merging

## Releases

Not applicable yet. Project is in early development.
