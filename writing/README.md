# ライティング作業ディレクトリ

セットアップ完了日: 2026-05-15

## ディレクトリ構成

```
writing/
├── drafts/           # 執筆中の原稿 (YYYY-MM-DD-<題名>.md)
├── research/         # 取材・調査資料 (<題名>/ サブディレクトリ)
├── final/            # 完成稿 (YYYY-MM-DD-<題名>.md)
├── published/        # 公開済みアーカイブ
├── templates/        # 記事テンプレート
│   └── article.md    # 汎用記事テンプレート
├── snippets/         # 定型文・常用フレーズ
├── tone/             # 媒体別トーン設定
│   └── _template.md  # トーン設定テンプレート
└── styleguide.md     # 表記ルール
```

## 関連ファイル

- **[CLAUDE.writer.md](../CLAUDE.writer.md)** — Claude への行動指針・ワークフロー定義
- **[memory/writing-knowledge/](../memory/writing-knowledge/)** — 蓄積されたノウハウ
- **[.company/secretary/notes/](../.company/secretary/notes/)** — 進捗記録

## クイックスタート

### 新しい記事を書き始める

1. `writing/drafts/YYYY-MM-DD-<題名>.md` を作成
2. `writing/templates/article.md` をコピーして企画メモを記入
3. 調査資料は `writing/research/<題名>/` に整理

### 媒体トーン設定を追加する

1. `writing/tone/_template.md` をコピー
2. ファイル名を `writing/tone/<媒体名>.md` として保存
3. 各項目を埋める

---

セットアップ完了。最初のタスクは何ですか？
