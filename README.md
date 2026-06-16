# Kusanali コミュニティ — 公開看板

Kusanali コミュニティ向けタスク看板。**正本は GitHub Projects**（このリポジトリ）。

## 看板 URL（正）

```bash
gh auth refresh -h github.com -s project,read:project
oc kanban setup
oc kanban url
```

## 列（Status）

| Status | 意味 |
|--------|------|
| Todo | 未着手 |
| In progress | 進行中 |
| Done | 完了 |
| Idea | アイデア |

## Issues（初回移行済み）

| # | 列 | タイトル |
|---|-----|----------|
| 1 | todo | エージェント更新手順を SKILL に追記 |
| 2–5 | done | Canvas / Discord / カンバン基盤 |
| 6–7 | idea | Discord スラッシュ / Canvas ギャラリー |

`oc kanban setup` で Project ボードに載る。

## エージェント

```bash
oc kanban list
oc kanban add "タイトル" --note "..." --column todo
oc kanban move 3 --to done
```

Docs: https://github.com/flll/openclaw/blob/main/services/kusanali-web/docs/KANBAN.md
