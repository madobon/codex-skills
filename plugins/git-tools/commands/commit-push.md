---
description: Create one intentional semantic commit for the current repository and push it to the tracked remote branch
argument-hint: [optional-scope]
allowed-tools: [Read, Glob, Grep, Bash, Write, Edit]
---

# Git Tools Commit Push

The user invoked this command with: $ARGUMENTS

When this command is invoked:

1. Read `skills/commit-push/SKILL.md`
2. Inspect the working tree before staging anything
3. Stage only the files that belong to one intentional commit
4. Create one semantic commit
5. Push to the tracked remote branch
6. Do not create a pull request

## Example Usage

```text
/git-tools:commit-push
/git-tools:commit-push update plugin metadata
```
