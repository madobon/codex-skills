---
name: semantic-commit
description: Use when the user wants the current uncommitted changes split into meaningful semantic commits instead of one large commit. Group related changes by intent, keep each commit coherent, and stop without pushing.
---

# Semantic Commit

## Workflow

1. Inspect the full diff and identify logical units of change.
2. Split changes only when each resulting commit remains buildable and understandable.
3. Commit in dependency order. Typical order is `refactor` before `feat`, `test`, or `fix` when that makes the history clearer.
4. Use semantic commit messages for every commit.
5. Stop after local commits are created.

## Guardrails

- If a safe split is unclear, prefer fewer commits.
- Never create a broken intermediate commit knowingly.
- Do not push.
- Do not rewrite existing commits.
