---
name: commit
description: Use when the user wants a single commit only in the current repository. Review the working tree, group the current changes into one intentional commit, write a concise semantic commit message, and stop without pushing.
---

# Commit

## Workflow

1. Inspect `git status --short` and `git diff --stat` before staging anything.
2. Read enough diff context to understand the user-facing intent.
3. Refuse to include clearly unrelated changes in the same commit. If the tree is mixed, ask the user or limit staging to the relevant paths.
4. Stage only the files that belong in this one commit.
5. Write a semantic commit message using a standard type such as `feat`, `fix`, `refactor`, `docs`, `test`, or `chore`.
6. Commit and report the resulting SHA.
7. Do not push.

## Guardrails

- Prefer one clean commit over speculative splitting.
- Do not rewrite history.
- Do not include generated lockfile noise unless it is required by the change.
