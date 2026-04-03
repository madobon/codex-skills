---
name: commit-push
description: Use when the user wants one commit and then a push for the current branch. Create a single intentional semantic commit, push it to the tracked remote, and stop without creating a pull request.
---

# Commit Push

Follow the `commit` workflow, then:

1. Confirm the current branch and upstream.
2. Push the new commit to the remote branch. If no upstream exists, push with `-u origin <branch>`.
3. Report the pushed branch and resulting commit SHA.

## Guardrails

- Do not create a PR.
- Do not use force push unless the user explicitly asks.
