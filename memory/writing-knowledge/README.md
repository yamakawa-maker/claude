# ライティング・ナレッジベース 運用ルール

このディレクトリはライティング業務で得た知見を蓄積する場所です。
`CLAUDE.writer.md` セクション 1.7 と同期して管理してください。

## カテゴリプレフィックス一覧

| プレフィックス | 用途 | ファイル例 |
|--------------|------|-----------|
| `style-` | 表記ルール変更履歴・媒体別判断 | `style-media-a-rules.md` |
| `phrase-` | 採用された秀逸な表現／避けたい表現 | `phrase-lead-openers.md` |
| `interview-` | 取材ノウハウ・質問テンプレ | `interview-startup-ceo.md` |
| `seo-` | 検索意図整理・キーワード設計 | `seo-target-keyword-map.md` |
| `trouble-` | 校正トラブル・差し戻し事例 | `trouble-factcheck-2026.md` |

## 蓄積タイミング

- 同じ指摘で2回目以上ハマったとき
- 媒体ごとの判断を確定したとき
- 公開後の反応からノウハウを抽出したとき

## タスク開始時のルール

タスク開始前に、関連するプレフィックスで `grep` して過去の知見を参照すること。

例:
```
grep -r "style-" ./memory/writing-knowledge/
```

## ファイル命名規則

```
<プレフィックス>-<内容を表すケバブケース>.md
```

例: `phrase-interview-closing.md`, `seo-saas-b2b-2026.md`
