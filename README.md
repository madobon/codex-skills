# codex-skills

個人用の Codex skill / plugin をまとめるリポジトリです。

現在は Git ワークフロー向けのローカル plugin `git-tools` を含んでいます。

- `git-tools:commit`
- `git-tools:commit-push`
- `git-tools:commit-push-pr`
- `git-tools:semantic-commit`
- `git-tools:semantic-cleanup`
- `git-tools:semantic-pr-cleanup`

## 構成

```text
plugins/
  git-tools/
.agents/
  plugins/
    marketplace.json
```

## ローカルで使う

home-local plugin として使う場合の配置は以下です。

1. このリポジトリを clone する
2. `plugins/git-tools` を `~/plugins/git-tools` に配置する
3. `~/.agents/plugins/marketplace.json` に `./plugins/git-tools` を指す marketplace entry を置く
4. Codex を再起動して plugin を有効化する

このリポジトリには repo-local 用の marketplace 定義として [`.agents/plugins/marketplace.json`](/Users/madobon/Projects/codex-skills/.agents/plugins/marketplace.json) も含めています。

重要なのは、home-local plugin の実体は `~/.codex/plugins/` ではなく `~/plugins/` に置くことです。

## 補足

`git-tools` はカスタムのスラッシュコマンドそのものではなく、`git-tools:commit` のようなプレフィックス付き skill として使う前提です。運用上は `/git-tools:commit` のような slash 風入力でも解釈できることがあります。
