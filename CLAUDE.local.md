# CLAUDE.local.md

**my-claude** は Claude Code の個人設定を管理するリポジトリです。`~/.claude` にシンボリックリンクを貼ることで、Claude Code に設定が適用されます。
このプロダクトの構造はClaude Codeの設定ファイルの構造に準拠するのでClaudeに関する既存知識や該当する最新ドキュメントを参考にできます。

## プロジェクト構成

### 1. サブエージェント (`agents/`)

公式ドキュメント: https://docs.claude.com/ja/docs/claude-code/sub-agents

### 2. スラッシュコマンド (`commands/`)

公式ドキュメント: https://docs.claude.com/ja/docs/claude-code/slash-commands

### 3. Claude Codeの設定全般 (`settings.json`)

公式ドキュメント: https://docs.claude.com/ja/docs/claude-code/settings
公式ドキュメント(フック設定など): https://docs.claude.com/ja/docs/claude-code/hooks

## その他参照すべきファイル

- ~/.claude.json
  - Claudeの設定やログが記載されたファイル
  - git管理されていないので編集する際は差分を提示して人間の許可を得るべき
