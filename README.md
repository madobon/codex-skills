# codex-skills

[![Codex](https://img.shields.io/badge/Codex-local%20plugins-111111?style=flat-square)](#)
[![Plugin](https://img.shields.io/badge/plugin-git--tools-14532D?style=flat-square)](#git-tools)
[![Skills](https://img.shields.io/badge/skills-6-blue?style=flat-square)](#git-tools)
[![License](https://img.shields.io/badge/license-MIT-0f766e?style=flat-square)](#)

個人用の Codex skill / plugin をまとめるリポジトリです。現在は Git ワークフローをまとめた local plugin `git-tools` を収録しています。

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
/git-tools:commit
/git-tools:commit-push
git-tools:semantic-pr-cleanup でやって
```

`git-tools` は組み込み slash command そのものではなく、`git-tools:commit` のような prefixed skill として使う前提です。運用上は `/git-tools:commit` のような slash 風入力でも解釈できることがあります。

## Layout

```text
plugins/
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
- `git-tools` の metadata は [`plugins/git-tools/.codex-plugin/plugin.json`](/Users/madobon/Projects/codex-skills/plugins/git-tools/.codex-plugin/plugin.json)
