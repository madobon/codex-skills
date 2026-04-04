---
description: Review the current repository changes, create one intentional semantic commit, and stop without pushing
argument-hint: [optional-scope]
allowed-tools: [Read, Glob, Grep, Bash, Write, Edit]
---

# Git Tools Commit

The user invoked this command with: $ARGUMENTS

When this command is invoked:

1. Read `skills/commit/SKILL.md`
2. Inspect the working tree before staging anything
3. Stage only the files that belong to one intentional commit
4. Create one semantic commit
5. Do not push

## Example Usage

```text
/git-tools:commit
/git-tools:commit fix auth tests
```
