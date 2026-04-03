---
name: semantic-cleanup
description: Use when the user has messy local changes and wants them cleaned up into a few meaningful semantic commits. This is a more conservative semantic commit mode focused on tidying scattered edits without rewriting history or pushing.
---

# Semantic Cleanup

Use this when the working tree contains mixed fixes, review comments, test updates, or incidental refactors.

## Workflow

1. Inspect the entire working tree and summarize the main change buckets.
2. Reduce noise first by separating formatting-only or generated changes from real behavior changes.
3. Create the smallest set of semantic commits that still explains the work clearly.
4. Prefer commit messages that make later review easy, such as `fix: address null handling in sync job` or `test: cover retry path`.
5. Stop after local commits are created.

## Guardrails

- Be conservative. Cleanup is for clearer history, not maximal fragmentation.
- Do not push.
- Do not rewrite existing commits.
