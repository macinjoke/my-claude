---
name: review-to-md
description: コードレビューをする
disable-model-invocation: true 
---

## Description

指定されたプルリクエストやコミットのコードを読み解き、概要のまとめとレビューをマークダウンに出力する。

プルリクの概要のまとめは: summary_{pull_request_id or commitId or timestamp}.md に書き出す。
レビューは: review_{pull_request_id or commitId or timestamp}.md に書き出す。

## Usage

- `/review-to-md {pull_request_url}`: 対象プルリクエストのレビューをする
- `/review-to-md {commitId}`: 対象のコミットのレビューをする
- `/review-to-md {フリーテキスト}` -> 文章を読み解き、対象のコードをレビューする
