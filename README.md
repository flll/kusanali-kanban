# Kusanali コミュニティ — 公開看板

Kusanali コミュニティ向けタスク看板。**正本は GitHub Projects**（このリポジトリの Project タブ）。

## 看板 URL（正）

<!-- PROJECT_URL: 作成後に oc kanban url で確認 -->

Project 作成後: `https://github.com/flll/kusanali-kanban/projects/<N>`

## 列（Status）

| Status | 意味 |
|--------|------|
| Todo | 未着手 |
| In progress | 進行中 |
| Done | 完了 |
| Idea | アイデア |

## タスク提案

1. [Issues](../../issues/new) で提案（ラベル `proposal` 推奨）
2. owner / エージェントが Project に追加・列を更新

## 載せないもの

- Tailscale IP / 100.x アドレス
- SSH ホスト名・鍵パス
- brain 内容・API トークン

## エージェント更新

OpenClaw / Cursor から:

```bash
oc kanban list
oc kanban add "タイトル" --note "説明" --column todo
oc kanban move 3 --to done
```

詳細: [openclaw KANBAN.md](https://github.com/flll/openclaw/blob/main/services/kusanali-web/docs/KANBAN.md)
