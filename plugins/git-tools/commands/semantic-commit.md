---
description: Clean up current changes into a semantic commit with stronger message discipline
argument-hint: [optional-scope]
allowed-tools: [Read, Glob, Grep, Bash, Write, Edit]
---

# Git Tools Semantic Commit

The user invoked this command with: $ARGUMENTS

When this command is invoked:

1. Read `skills/semantic-commit/SKILL.md`
2. Inspect the current changes
3. Create a semantic commit that matches the actual change scope
4. Do not push unless the skill says to

## Example Usage

```text
/git-tools:semantic-commit
/git-tools:semantic-commit docs cleanup
```
