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

このリポジトリを clone したうえで、`.agents/plugins/marketplace.json` の plugin 定義をローカルの Codex から参照します。

シンプルに使うだけなら、`plugins/git-tools` を `~/.codex/plugins/` 配下へコピーしても構いません。

## 補足

`git-tools` はカスタムのスラッシュコマンドではなく、`git-tools:commit` のようなプレフィックス付き skill として使う前提です。
