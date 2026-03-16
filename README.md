# AI Work Basement

このリポジトリは、AIを使った業務ドキュメントを手早く立ち上げるためのテンプレートです。

## 簡単な構造

```
.
├── README.md                   : この文書
├── AGENTS.md.sample            : AIエージェントと仕事する際の初期命令
├── bin                         : 便利コマンド群
│   └── init                    : └─ つかいはじめる際の初期化
├── docs                        : AIエージェントと対話して作業をするためのコンテキスト群
│   ├── 0_WHITEBOARD.md         : ├─ やりたいことをとにかく書き起こす場所
│   ├── 1_PITCH.md              : ├─ やりたいことを簡単な企画書にした形
│   ├── 2_PLAN.md               : ├─ PITCHを基にした作業計画書
│   ├── 3_TODO.md               : ├─ 作業のTODOの一覧と進捗状況管理
│   ├── 4_CHECKPOINT.md         : ├─ AIとの作業セッションごとの経過記録
│   └── 9_KNOWLEDGEMENT.md      : └─ 参照すべき情報の記載
├── attachments                 : AIに参照させたいファイルの置き場所
└── outputs                     : 出力ファイルの置き場
    └── AI-CONVERSATION-LOG.md  : └─ AIとの会話ログ（セッションごとの記録）

```

## つかいかた

1. このリポジトリをcloneする。
2. bin/init を実行して、別リポジトリに変換する。
3. AGENTS.md.sampleを基にAIエージェントの姿勢を定義する。
4. 作業計画をはじめる。
5. AIとの会話の要点・決定事項・次のアクションは `outputs/AI-CONVERSATION-LOG.md` に自動で記録される。

## 会話ログについて

`outputs/AI-CONVERSATION-LOG.md` はAIとの会話をそのまま記録するファイルです。
AIエージェントは各ターンの発言・返答を要約せずそのままこのファイルに自動追記します。
指示がなくても記録されるため、会話の全文をいつでも参照できます。
