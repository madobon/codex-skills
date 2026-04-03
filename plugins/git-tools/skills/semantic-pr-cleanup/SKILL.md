---
name: semantic-pr-cleanup
description: Use when the user is updating an existing PR branch after review or follow-up fixes and wants the remaining local changes organized into meaningful semantic commits. Clean up the pending changes, commit them coherently, and push the branch to update the PR.
---

# Semantic PR Cleanup

Use this on an existing PR branch after review feedback, test fixes, or follow-up edits have accumulated locally.

## Workflow

1. Inspect `git status`, branch tracking, and the diff against the remote branch.
2. Identify review-response buckets such as bug fixes, tests, docs, or small refactors.
3. Create a few coherent semantic commits for the pending changes.
4. Push the branch to update the existing PR.
5. Report the new commit SHAs and branch name.

## Guardrails

- This mode organizes pending local changes only.
- Do not rewrite existing commits or use force push unless the user explicitly asks.
- If there is no tracked remote branch, set one up during push and report it.
