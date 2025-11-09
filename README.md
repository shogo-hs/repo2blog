# repo2blog

このリポジトリは `target_repository/` 以下の各OSSを読み解き、技術ブログ記事を `output_docs/` 配下に生成するためのワークスペースです。

## ディレクトリ構成
- `AGENTS.md` : 執筆ルールやターゲット読者などの指示書
- `target_repository/` : リサーチ対象となるGitHubリポジトリ（※ `.gitignore` 済）
  - 例: `toon-python/`
- `output_docs/` : 完成したブログ記事（Markdown）を置く場所
- `README.md` : 本書（セットアップおよび作業手順の概要）

## 使い方
1. `AGENTS.md` を確認し、章立てや必須要件を把握する。
2. `target_repository/<project>` を調査し、README・docs・srcなどを読み込む。
3. `output_docs/<project>.md` に日本語で記事を書く。必要に応じてMermaid図やコード片を追加。
4. 仕上げとして `git add output_docs/<project>.md` などでコミットする。

## 注意事項
- 対象レポジトリはサイズが大きいため `target_repository/` をGit管理から除外しています。
- 記事には最終更新日・バージョン・引用元ファイルなど、`AGENTS.md` に記載のMUST要件を忘れずに含めてください。
