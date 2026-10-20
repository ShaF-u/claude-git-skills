# claude-git-skills

Git 操作用の Claude Code スキル。手動起動専用（`disable-model-invocation: true`）なので、勝手にコミット・プッシュされない。

| コマンド | 内容 |
|---|---|
| `/git-commit [ヒント] [--no-push]` | ドキュメントを同期してから全変更をコミットし、プッシュ |
| `/git-branches [--offline]` | ローカル・リモートのブランチ一覧と追跡状態、stash、worktree |
| `/git-sync` | 上流から fetch して fast-forward（サブモジュールも更新） |

ブランチの作成・切替・force push はしない。

## インストール

```
claude plugin marketplace add ShaF-u/claude-git-skills
claude plugin install git-skills@git-skills
```

コマンドは `/git-skills:git-commit` の形になる（`/git-commit` と打てば補完される）。

元は `ShaF-u/claude-spec-kit` に入っていたもの（03f466a で分離）。
