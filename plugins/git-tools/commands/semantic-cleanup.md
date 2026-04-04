---
description: Clean up follow-up changes after feedback and commit them with a precise semantic message
argument-hint: [optional-scope]
allowed-tools: [Read, Glob, Grep, Bash, Write, Edit]
---

# Git Tools Semantic Cleanup

The user invoked this command with: $ARGUMENTS

When this command is invoked:

1. Read `skills/semantic-cleanup/SKILL.md`
2. Inspect the current follow-up changes
3. Group only the cleanup-related changes
4. Commit them with a precise semantic message

## Example Usage

```text
/git-tools:semantic-cleanup
/git-tools:semantic-cleanup address review nits
```
