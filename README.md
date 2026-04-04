# codex-skills

[![Codex](https://img.shields.io/badge/Codex-local%20plugins-111111?style=flat-square)](#)
[![Plugins](https://img.shields.io/badge/plugins-2-14532D?style=flat-square)](#frontend-design)
[![Skills](https://img.shields.io/badge/skills-7-blue?style=flat-square)](#frontend-design)
[![License](https://img.shields.io/badge/license-MIT-0f766e?style=flat-square)](#)

個人用の Codex skill / plugin をまとめるリポジトリです。現在は Git ワークフローをまとめた local plugin `git-tools` と、UI 実装向けの `frontend-design` を収録しています。

## Frontend Design

Frontend Design は、ページ、コンポーネント、ダッシュボード、ランディングページなどの見た目を Codex で作り込むための plugin です。

### Available Skills

- `frontend-design:frontend-design`

### Quick Start

home-local plugin として使う場合は、`plugins/frontend-design` を `~/plugins/frontend-design` に配置し、`~/.agents/plugins/marketplace.json` に `./plugins/frontend-design` を指す entry を追加します。

### Example

```text
Use frontend-design:frontend-design to redesign this React settings page.
Use frontend-design:frontend-design to build a bold landing page for a cafe.
```

## Git Tools

Git Tools は、commit、push、PR 前後の cleanup をまとめて扱うための plugin です。

### Available Skills

- `git-tools:commit`
- `git-tools:commit-push`
- `git-tools:commit-push-pr`
- `git-tools:semantic-commit`
- `git-tools:semantic-cleanup`
- `git-tools:semantic-pr-cleanup`

### Quick Start

home-local plugin として使う場合は、次の形に揃えるのが一番安定します。

1. このリポジトリを clone する
2. `plugins/git-tools` を `~/plugins/git-tools` に配置する
3. `~/.agents/plugins/marketplace.json` に `./plugins/git-tools` を指す marketplace entry を置く
4. Codex を再起動して plugin を有効化する

重要なのは、plugin の実体を `~/.codex/plugins/` ではなく `~/plugins/` に置くことです。

### Example

```text
Use git-tools:commit for the current repository.
Use git-tools:commit-push on this branch.
Use git-tools:semantic-pr-cleanup for this PR branch.
```

`git-tools` は plugin に含まれる prefixed skill として使う前提です。

## Layout

```text
plugins/
  frontend-design/
    .codex-plugin/plugin.json
    plugin.lock.json
    assets/
    skills/
  git-tools/
    .codex-plugin/plugin.json
    plugin.lock.json
    assets/
    skills/
.agents/
  plugins/
    marketplace.json
```

repo-local 用の marketplace 定義は [`.agents/plugins/marketplace.json`](/Users/madobon/Projects/codex-skills/.agents/plugins/marketplace.json) にあります。

## Notes

- home-local plugin の marketplace は `~/.agents/plugins/marketplace.json`
- home-local plugin の実体パスは `~/plugins/<plugin-name>`
- `frontend-design` の metadata は [`plugins/frontend-design/.codex-plugin/plugin.json`](/Users/madobon/Projects/codex-skills/plugins/frontend-design/.codex-plugin/plugin.json)
- `git-tools` の metadata は [`plugins/git-tools/.codex-plugin/plugin.json`](/Users/madobon/Projects/codex-skills/plugins/git-tools/.codex-plugin/plugin.json)
