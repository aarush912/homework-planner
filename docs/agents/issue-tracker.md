# Issue tracker: GitHub

Issues and specs for this repo live as GitHub issues. Use the `gh` CLI for all operations.

## Conventions

- Create: `gh issue create --title "..." --body "..."`.
- Read: `gh issue view <number> --json number,title,body,labels,comments`.
- List: `gh issue list --state open --json number,title,body,labels,comments`.
- Comment: `gh issue comment <number> --body "..."`.
- Apply or remove labels: `gh issue edit <number> --add-label "..."` / `--remove-label "..."`.
- Close: explain with `gh issue comment`, then run `gh issue close <number>`.
- Infer the repo from `git remote -v`; `gh` does this automatically inside a clone.
- File issues only in the user's own repo. Before the first issue creation in a session, verify the target with `gh repo view --json nameWithOwner`.

## Pull requests as a triage surface

**PRs as a request surface: no.**

## When a skill says "publish to the issue tracker"

Create a GitHub issue.

## When a skill says "fetch the relevant ticket"

Read it with `gh issue view`.

## Wayfinding operations

Use a map issue labeled `wayfinder:map`, with child issues as tickets. Link children as GitHub sub-issues where available; otherwise use a task list in the map and put `Part of #<map>` at the top of each child. Use `wayfinder:<type>` labels (`research`, `prototype`, `grilling`, `task`). Claim with `gh issue edit <n> --add-assignee @me`; resolve by commenting, closing, and adding the context pointer to the map.
