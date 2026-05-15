# Claude Code — ライティング業務設定リポジトリ

ライター向け Claude Code 環境の設定・テンプレート・ナレッジを一元管理するリポジトリです。

---

## ファイル構成

```
/
├── CLAUDE.md                        # Claude への指示（エントリーポイント）
├── CLAUDE.writer.md                 # Claude 詳細設定（役割・ワークフロー・制約）
│
├── writing/                         # 原稿・資料置き場
│   ├── drafts/                      # 執筆中の原稿
│   ├── research/                    # 取材・調査資料
│   ├── final/                       # 完成稿
│   ├── published/                   # 公開済みアーカイブ
│   ├── templates/
│   │   └── article.md               # 汎用記事テンプレート
│   ├── snippets/                    # 定型文・常用フレーズ
│   ├── tone/
│   │   └── _template.md             # 媒体別トーン設定テンプレート
│   └── styleguide.md                # 表記ルール
│
├── memory/
│   └── writing-knowledge/           # 蓄積ナレッジ（プレフィックス管理）
│       └── README.md                # カテゴリ・運用ルール
│
└── .company/
    └── secretary/
        └── notes/                   # 進捗記録（日次）
```

---

## クイックリファレンス

### 新しい記事を始める

```
writing/drafts/YYYY-MM-DD-<題名>.md  ← writing/templates/article.md をコピーして使用
writing/research/<題名>/             ← 調査資料・取材ログをここに
```

### 媒体トーン設定を追加する

```
writing/tone/_template.md をコピー → writing/tone/<媒体名>.md として保存
```

### ナレッジを蓄積する

```
memory/writing-knowledge/<プレフィックス>-<内容>.md
```

| プレフィックス | 用途 |
|---|---|
| `style-` | 表記ルール変更履歴・媒体別判断 |
| `phrase-` | 採用された表現／避けたい表現 |
| `interview-` | 取材ノウハウ・質問テンプレ |
| `seo-` | 検索意図整理・キーワード設計 |
| `trouble-` | 校正トラブル・差し戻し事例 |

---

## 設定ファイル早見表

| ファイル | 用途 | 更新頻度 |
|---------|------|----------|
| [CLAUDE.md](CLAUDE.md) | Claude への基本指示 | 設定変更時 |
| [CLAUDE.writer.md](CLAUDE.writer.md) | Claude 詳細設定 | 設定変更時 |
| [writing/styleguide.md](writing/styleguide.md) | 表記ルール | 媒体追加・ルール確定時 |
| [writing/templates/article.md](writing/templates/article.md) | 記事テンプレート | テンプレ改訂時 |
| [writing/tone/_template.md](writing/tone/_template.md) | 媒体トーン設定テンプレート | テンプレ改訂時 |
| [memory/writing-knowledge/README.md](memory/writing-knowledge/README.md) | ナレッジ運用ルール | 運用変更時 |

---

## 原稿ライフサイクル

```
drafts/ → (推敲) → final/ → (公開後) → published/
```

公開後は `published/` 内ファイルの冒頭に公開URL・公開日・媒体名を追記する。
