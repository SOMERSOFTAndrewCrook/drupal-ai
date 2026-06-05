---
name: workflow
description: Git and PR workflow conventions — branch naming, commit messages, PR process, and base branch
---

# Workflow Rules

> Replace `PRJ` with your project's actual Jira key (e.g. `MYAPP`, `WEB`, `ACME`).

## Base Branch

- Main branch is `develop` — all feature branches are cut from and merged back into `develop`
- `main` is the production/release branch — do not target it for PRs unless explicitly instructed

## Branch Naming

Format: `PRJ-XXX-short-description`

- Prefix with the Jira ticket ID
- Lowercase, hyphens only
- Keep the description short and meaningful

Examples:
- `PRJ-356-lucidworks-indexing-endpoints`
- `PRJ-808-accordion-overflow-fix`

## Commit Messages

Format: `PRJ-XXX: Short imperative description`

- Prefix with the Jira ticket ID followed by a colon
- Use imperative mood ("Add", "Fix", "Update" — not "Added", "Fixed")
- Keep the first line concise

Examples:
- `PRJ-356: Add Lucidworks indexing endpoints`
- `PRJ-808: Fix accordion overflow with shadow indicator`

## Pull Requests

- PR title should mirror the commit message format: `PRJ-XXX: Description`
- Target `develop` unless otherwise specified
- Link the Jira ticket in the PR body
- Use the `/ready-pr-in-review` command to move a PR through the review workflow
