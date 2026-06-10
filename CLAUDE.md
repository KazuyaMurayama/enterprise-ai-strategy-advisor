# Enterprise AI Strategy Advisor — Claude Code 運用ルール

企業の AI 活用戦略を立案・評価・ロードマップ化する AI コンサルタントシステム。業界・組織規模・現状課題を入力すると、具体的なAI導入施策と優先順位を自動生成する。

> **本ファイルは VSCode版 / Web版 Claude Code（claude.ai）の両方で本リポジトリの単独完結ガイド**。
> Web版はグローバル `~/.claude/CLAUDE.md` を参照しない前提で、本リポの運用に必要な全ルールをここに集約。

---

## 0. プロジェクト主機能
- 業界別 AI 活用事例データベース参照
- ROI 試算・費用対効果シミュレーション
- 組織の AI 成熟度診断
- 導入ロードマップ自動生成
- 経営層向けエグゼクティブサマリー作成

---

## 1. セッション開始時の参照順序
1. `tasks.md` — タスク管理・セッション履歴（存在する場合）
2. `FILE_INDEX.md` — ファイル一覧インデックス（存在する場合）
3. このCLAUDE.md — ルール入口

---

## 2. 関連リポジトリ
| リポ | 役割 |
|---|---|
| [KazuyaMurayama/AI-Transformation-Architect](https://github.com/KazuyaMurayama/AI-Transformation-Architect) | 企業 AI 変革支援本体 |
| [KazuyaMurayama/AI-ROI-simulator_v1](https://github.com/KazuyaMurayama/AI-ROI-simulator_v1) | ROI/NPV/回収期間試算 |
| [KazuyaMurayama/AI-Architect-forge_v1](https://github.com/KazuyaMurayama/AI-Architect-forge_v1) | アーキテクチャ設計・評価 |

---

## 3. 開発者情報・命名ルール

| 種別 | 表記 | 用途 |
|---|---|---|
| **システム識別子（変更不可）** | `KazuyaMurayama` | GitHub ユーザー名 / URL / `@KazuyaMurayama` |
| **システム識別子（変更不可）** | `kazuya.murayama.21@gmail.com` | git `user.email` / 連絡先 |
| **表記名（人間として記載する場合）** | **男座員也（Kazuya Oza / おざ かずや）** | ドキュメント本文の著者名 / コミット message 中の自己言及 |

- ドキュメント本文・コード・コミットメッセージ本文等で開発者名を**人間として**記載する際は **男座員也 / Kazuya Oza** を使用
- 「Murayama」「村山」「Otokoza」「おとこざ」を**表記名**として誤用しない（システム識別子としての `KazuyaMurayama` は許容）

---

## 4. ツール実行・Shell・Git・ファイル保存
- 確認不要・即実行（事前確認文を出力しない）
- ファイル操作は Edit/Write/Read/Grep/Glob を直接使用
- 例外（事前確認必須）: main への `git push --force`、`gh repo delete`
- Shell: VSCode版は Windows 11 + PowerShell 5.1（`&&` 不可 → `;` + `if ($?)`）/ Bash併用可。Web版は Linux サンドボックス
- **ブランチ管理**: デフォルトはmainへ直接コミット。ブランチ作成は明示指示時のみ。万一作成した場合は必ずmainマージ→削除→push完了で「完了」
- **ファイル保存**: 本リポ内のみ。`C:\Users\user\Desktop` への出力禁止

---

## 5. 成果物報告ルール（最重要・毎回必須）

| 成果物 | 説明 | リンク |
|---|---|---|
| file.md | 1行説明 | [開く](https://github.com/KazuyaMurayama/enterprise-ai-strategy-advisor/blob/main/path/to/file.md) |

- Markdownリンク `[表示名](URL)` 形式必須
- `/blob/<実ブランチ>/<実パス>` 形式
- **報告前にURL存在確認**：`Invoke-WebRequest -Uri https://api.github.com/repos/KazuyaMurayama/enterprise-ai-strategy-advisor/contents/PATH?ref=BRANCH -UseBasicParsing` でステータス200確認
- ブランチ名は推測禁止：`git rev-parse --abbrev-ref HEAD`
- push完了後のみURL生成

---

## ドキュメント命名・日付ルール（v2.0 / 2026-06-03 改訂）

### ファイル名
- `<TOPIC>_YYYYMMDD.md` 形式（**サフィックス・ハイフンなし**）
  - 例: `STRATEGY_REPORT_20260603.md`
- **同日中の追加更新**: `-v2`、`-v3` を追加（例: `STRATEGY_REPORT_20260603-v2.md`）
- **翌日1回目**: v サフィックスをリセット（例: `STRATEGY_REPORT_20260604.md`）

### 表記の区別
- **ファイル名**: ハイフン**なし** `YYYYMMDD`（例: `20260603`）
- **本文中の日付表記**: ハイフン**あり** `YYYY-MM-DD`（例: `2026-06-03`）

### H1直下の日付メタデータ
レポート系 .md 新規作成時は H1直下に必ず記載:
```
作成日: YYYY-MM-DD
最終更新日: YYYY-MM-DD
```
更新時は **最終更新日のみ** 当日付に書き換え（作成日は固定）。

### 対象外（日付サフィックスを入れない）
- README / CLAUDE.md / FILE_INDEX / tasks.md / CHANGELOG / LICENSE / SPEC.md
- `CURRENT_*.md`（常に最新で参照される単一ファイル）
- パイプライン自動生成ファイル（例: `REPORT.md`、`outputs/*.md`）

### 旧形式（廃止・新規禁止）
- ❌ `<TOPIC>_2026-06-03.md`（ハイフン区切り）
- ✅ `<TOPIC>_20260603.md`（**現行ルール**）

---

## 7. Skill 起動ルール（必須・スキップ禁止）
該当シーンでは `.claude/skills/<name>/SKILL.md` を読んでから作業を開始する。

| トリガー | スキル |
|---|---|
| 戦略レポート・事業分析・提案書 | `.claude/skills/management-consulting/SKILL.md` |
| 業界事例・先行事例の調査 | `.claude/skills/research-deep/SKILL.md` |
| ROI/インパクト定量化 | `.claude/skills/impact-quantification/SKILL.md` / `business-metrics-calculator/SKILL.md` |
| 経営層向けサマリー | `.claude/skills/executive-summary-generator/SKILL.md` |
| 技術成果のビジネス翻訳 | `.claude/skills/technical-to-business-translator/SKILL.md` |
| ステークホルダー要件 | `.claude/skills/stakeholder-requirements-gathering/SKILL.md` |
| 図表生成 | `.claude/skills/mermaid-agents365/SKILL.md` |
| QC・レビュー前 | `.claude/skills/analysis-qa-checklist/SKILL.md` |
| 成果物の納品・コミット前 | `.claude/skills/sp-verification-before-completion/SKILL.md` |
| 計画立案 | `.claude/skills/sp-writing-plans/SKILL.md` + `sp-executing-plans/SKILL.md` |

---

## モデル使い分け
- メイン: **Claude Fable 5（`claude-fable-5`）** を使用。
  計画・中〜高難易度の実装/分析・全体指揮を担当。
- 実行フェーズ（定型実装・ファイル編集・テスト実行）:
  サブエージェントを `model: "sonnet"` で起動して委譲。
- ※難易度ベースの自動メイン切替は不可。Fable の自動切替は安全性ブロック時の
  Opus 4.8 フォールバックのみ。工程別の使い分けはサブエージェント委譲で行う。
