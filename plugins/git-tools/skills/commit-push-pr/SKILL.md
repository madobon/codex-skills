---
name: commit-push-pr
description: Use when the user wants one commit, a push, and pull request creation. Create one intentional semantic commit, push the branch, and open a PR with a concise title and body.
---

# Commit Push PR

Follow the `commit-push` workflow, then:

1. Determine the base branch from the repository default or existing branch context.
2. Create a PR with `gh pr create` when one does not already exist for the branch.
3. Generate a semantic PR title aligned with the commit intent.
4. Write a short PR body with summary, testing, and any follow-up notes.
5. Report the PR URL.

## Guardrails

- If a PR already exists, update the branch by pushing and report the existing PR instead of creating a duplicate.
- Do not squash or rewrite history unless the user explicitly asks.
