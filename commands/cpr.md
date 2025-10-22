---
name: cpr
description: 現在のブランチを push して GitHub PR を作成する
---

## Description
このコマンドは以下の作業を自動で実行します：
1. 現在のブランチを `git push` する
2. コミットメッセージやコミットログからブランチの修正・実装内容を理解しまとめる
3. 内容を簡潔にまとめた一文をPRタイトルに利用
3. base ブランチとの差分内容をPR本文に利用
4. GitHub CLI (`gh`) を用いて PR を作成する

## Usage
- `/cpr develop` → develop 向け PR を作成
- `/cpr main` → main 向け PR を作成（hotfix 用）
- `/cpr [ブランチ名]` -> 特定のブランチに向けて PR を作成

## Implementation
- git操作
  - ghコマンドが利用できればghコマンドを利用する
  - なければmcpを利用する

