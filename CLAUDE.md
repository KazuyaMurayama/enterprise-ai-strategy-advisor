# Enterprise AI Strategy Advisor

## プロジェクト概要
企業名または業界名を入力するだけで、MBB（マッキンゼー・ベイン・BCG）クラスの生成AI戦略レポートを自動生成するシステム。

## FILE_INDEX.md 参照ルール

**`FILE_INDEX.md`** は以下のタイミングで必ず参照すること：

1. **セッション開始時** — ファイル構成・ブランチ状態・生成済みレポートの概要を把握する
2. **これまでの経緯・最新状態を確認すべき時** — バージョン差分・レポート更新履歴を確認する
3. **ファイル参照指示があった時** — 該当ファイルのパス・最新版を特定してから作業する

---

## 品質基準
- **マッキンゼー水準**: MECE構造化、定量インパクト試算、So What?の明確化
- **ベイン水準**: 実行可能性重視の具体的アクションプラン、ROI試算、Full Potential分析
- **BCG水準**: フレームワーク活用（バリューチェーン分析、成熟度モデル、アンビション・マトリクス）
- 数値根拠のない主張は禁止。推定でもロジックと前提を明示（フェルミ推定可）

> プライオリティマトリクスを生成する時は `.claude/rules/priority-matrix.md` を読む

> AIセキュリティ・ガバナンス章を記述する時は `.claude/rules/security-framework.md` を読む

> レポート生成・スキルコマンド・エージェントチームの詳細は `.claude/rules/report-workflow.md` を読む

## 開発者情報・命名ルール

このリポジトリの開発者・所有者は **男座員也（Kazuya Oza / おざ かずや）** です。

- ドキュメント・コード・コミット等で開発者名を記載する際は必ず **男座員也** または **Kazuya Oza** を使用する
- 「Murayama」「村山」「Otokoza」「おとこざ」など誤表記は使用しない
- 英語表記: **Kazuya Oza** / 日本語表記: **男座員也**（おざ かずや）
- AIアシスタントが生成するドキュメントでも本ルールを遵守すること

## ファイル保存ルール
- 成果物・スクリプトは本リポジトリ内のみに保存。`C:\\Users\\user\\Desktop` への出力禁止（ユーザー明示指定時を除く）。

<!-- SKILLS_RULES_START -->
## Skill 起動ルール（v2.1 / 2026-05-29）
以下のスキルは **必須・スキップ禁止**。該当シーンでは SKILL.md を読んでから作業を開始すること。

- **戦略レポート・事業分析・提案書を作成する時は必ず** `.claude/skills/management-consulting/SKILL.md` を読み、McKinsey/BCG/Bain 水準のフレームワークに従って作成する
- **市場・競合・先行研究の調査が必要な時は必ず** `.claude/skills/research-deep/SKILL.md` を読んでから並列 Web リサーチを実行する
- **資料・レポートに図表が必要な時は必ず** `.claude/skills/mermaid-agents365/SKILL.md` を読んでからダイアグラムを作成する
- **提案書・計画書の構成を考える前に必ず** `.claude/skills/sp-writing-plans/SKILL.md` を読んで構成を設計し、`.claude/skills/sp-executing-plans/SKILL.md` の手順で実行する
- **成果物の納品・コミット前、または品質チェック（QC）・レビューフェーズに入る時は必ず** `.claude/skills/sp-verification-before-completion/SKILL.md` のチェックリストを実行する
- **分析・レポートの品質チェック（QC）・レビュー・共有前は必ず** `.claude/skills/analysis-qa-checklist/SKILL.md` を読んでチェックリストを実施する
- **提案書・戦略レポートのピアレビューを実施する時は必ず** `.claude/skills/peer-review-template/SKILL.md` を読んでレビューを実施する
<!-- SKILLS_RULES_END -->
