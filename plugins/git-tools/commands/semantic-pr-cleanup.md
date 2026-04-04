---
description: Clean up PR follow-up changes, commit them semantically, and preserve a tidy branch history
argument-hint: [optional-scope]
allowed-tools: [Read, Glob, Grep, Bash, Write, Edit]
---

# Git Tools Semantic PR Cleanup

The user invoked this command with: $ARGUMENTS

When this command is invoked:

1. Read `skills/semantic-pr-cleanup/SKILL.md`
2. Inspect the current PR follow-up changes
3. Group only the cleanup-related changes
4. Commit them with a precise semantic message
5. Follow the skill guidance for PR cleanup work

## Example Usage

```text
/git-tools:semantic-pr-cleanup
/git-tools:semantic-pr-cleanup address latest review
```
