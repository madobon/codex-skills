---
description: Create one intentional semantic commit, push the branch, and prepare a pull request flow
argument-hint: [optional-scope]
allowed-tools: [Read, Glob, Grep, Bash, Write, Edit]
---

# Git Tools Commit Push PR

The user invoked this command with: $ARGUMENTS

When this command is invoked:

1. Read `skills/commit-push-pr/SKILL.md`
2. Inspect the working tree before staging anything
3. Stage only the files that belong to one intentional commit
4. Create one semantic commit
5. Push the branch
6. Continue with the PR workflow described in the skill

## Example Usage

```text
/git-tools:commit-push-pr
/git-tools:commit-push-pr prepare plugin release
```
