# Enterprise AI Strategy Advisor — ファイルインデックス

> **Claude Code 参照ルール**: ファイルを検索・参照する際は、**必ずこのインデックスを最初に確認**すること。  
> 同種ファイルが複数存在する場合、**日付（`_YYYYMMDD`）が新しいファイルが最新情報**を持つ。  
> スキルコマンドのルーティングは `CLAUDE.md` を参照。

---

## ブランチ一覧

| ブランチ名 | 最終コミット日 | 用途 |
|-----------|--------------|------|
| `claude/summarize-repos-sonnet-wkEJN` | 2026-04-14 | **インデックス整備済みブランチ（現在）** |
| `claude/ai-strategy-generator-hmKWX` | 2026-04-13 | 日本製造業AIレポート・AIセキュリティ 10領域フレームワーク |
| `claude/ai-strategy-pharma-No48g` | 2026-04-14 | 製薬業界3社レポート（大塔製薬・日本化薬・大樹生命） |

---

## 設定・システムファイル

| ファイルパス | 最終更新日 | サイズ | 説明 |
|-------------|-----------|-------|------|
| `CLAUDE.md` | 2026-04-13 | 7.1KB | **メイン設定** — 品質基準・AIセキュリティ10領域・コマンド一覧 |
| `FILE_INDEX.md` | 2026-04-14 | — | **本ファイル** — ナビゲーション起点 |
| `templates/report-template.md` | 2026-04-05 | 6.6KB | レポートテンプレート（オリジナル） |
| `templates/report-template_20260405.md` | 2026-04-05 | 6.6KB | レポートテンプレート（日付付き版） |

---

## スキルファイル（`.claude/skills/`）

> コマンド実行時のみ参照。日付なしが現行動作ファイル、日付付きが版管理用。

| ファイルパス | 最終更新日 | サイズ | 対応コマンド | 優先度 |
|-------------|-----------|-------|------------|--------|
| `.claude/skills/ai-strategy-full.md` | 2026-04-06 | 9.0KB | `/ai-strategy-full` | ★推奨 |
| `.claude/skills/ai-strategy-full_20260406.md` | 2026-04-06 | 9.0KB | 同上（日付付き版） | — |
| `.claude/skills/ai-strategy.md` | 2026-04-05 | 2.9KB | `/ai-strategy` | 標準 |
| `.claude/skills/ai-strategy_20260405.md` | 2026-04-05 | 2.9KB | 同上（日付付き版） | — |
| `.claude/skills/executive-summary.md` | 2026-04-05 | 1.4KB | `/executive-summary` | 単体 |
| `.claude/skills/executive-summary_20260405.md` | 2026-04-05 | 1.4KB | 同上（日付付き版） | — |
| `.claude/skills/industry-analysis.md` | 2026-04-05 | 1.8KB | `/industry-analysis` | 単体 |
| `.claude/skills/industry-analysis_20260405.md` | 2026-04-05 | 1.8KB | 同上（日付付き版） | — |
| `.claude/skills/roi-calculator.md` | 2026-04-05 | 1.9KB | `/roi-calculator` | 単体 |
| `.claude/skills/roi-calculator_20260405.md` | 2026-04-05 | 1.9KB | 同上（日付付き版） | — |
| `.claude/skills/usecase-mapper.md` | 2026-04-05 | 1.7KB | `/usecase-mapper` | 単体 |
| `.claude/skills/usecase-mapper_20260405.md` | 2026-04-05 | 1.7KB | 同上（日付付き版） | — |

---

## 生成済みレポート — ブランチ: `claude/ai-strategy-generator-hmKWX`

### 日本製造業（`output/japanese_manufacturing/`）

> **注**: Phase4・Phase8はAIセキュリティ10領域フレームワーク適用済み（2026-04-13更新）

| ファイルパス | 最終更新日 | サイズ | 内容 |
|-------------|-----------|-------|------|
| `output/japanese_manufacturing/README.md` | 2026-04-05 | 4.8KB | 目次・KPIサマリー |
| `output/japanese_manufacturing/full_report.md` | **2026-04-13** | 162KB | **統合レポート（最新・セキュリティ強化版）** |
| `output/japanese_manufacturing/phase1_executive_summary.md` | 2026-04-05 | 9.1KB | エグゼクティブサマリー |
| `output/japanese_manufacturing/phase2_industry_analysis.md` | 2026-04-05 | 21KB | 業界分析（PESTEL・Porter's 5 Forces） |
| `output/japanese_manufacturing/phase3_usecase_mapping.md` | 2026-04-05 | 25KB | バリューチェーンAI機会マッピング |
| `output/japanese_manufacturing/phase4_technology_architecture.md` | **2026-04-13** | 24KB | 技術アーキテクチャ ← セキュリティ4領域追加 |
| `output/japanese_manufacturing/phase5_organization_talent.md` | 2026-04-05 | 19KB | 組織・人材戦略 |
| `output/japanese_manufacturing/phase6_financial_model.md` | 2026-04-05 | 23KB | 財務モデル・ROI試算 |
| `output/japanese_manufacturing/phase7_roadmap.md` | 2026-04-05 | 23KB | 実行ロードマップ（36ヶ月） |
| `output/japanese_manufacturing/phase8_risk_management.md` | **2026-04-13** | 29KB | リスク管理 ← AIセキュリティ6領域追加 |
| `output/japanese_manufacturing/presentation_deck.md` | 2026-04-05 | 24KB | 経営層向け 20枚スライド |
| `output/japanese_manufacturing/ai_strategy_presentation.pptx` | 2026-04-05 | 65KB | PPTXファイル |

#### クライアントレビュー（`output/japanese_manufacturing/reviews/`）

| ファイルパス | 最終更新日 | サイズ | 内容 |
|-------------|-----------|-------|------|
| `output/japanese_manufacturing/reviews/client_a_cfo.md` | 2026-04-05 | 4.5KB | CFO視点クライアントレビュー |
| `output/japanese_manufacturing/reviews/client_b_cto.md` | 2026-04-05 | 5.6KB | CTO視点クライアントレビュー |
| `output/japanese_manufacturing/reviews/client_c_manufacturing.md` | 2026-04-05 | 5.7KB | 製造業担当者視点クライアントレビュー |

---

## 生成済みレポート — ブランチ: `claude/ai-strategy-pharma-No48g`

### 大塔製薬（`output/otsuka_pharma/`） ★最新

> ROI 257%・NPV 470億円・総投資350億円。GxP準拠・CNS創薬AI特化。

| ファイルパス | 最終更新日 | サイズ | 内容 |
|-------------|-----------|-------|------|
| `output/otsuka_pharma/README.md` | 2026-04-14 | 2.8KB | 目次（KPIサマリー） |
| `output/otsuka_pharma/full_report.md` | 2026-04-14 | 72KB | **統合レポート** |
| `output/otsuka_pharma/phase1_executive_summary.md` | 2026-04-14 | 5.6KB | エグゼクティブサマリー |
| `output/otsuka_pharma/phase2_industry_analysis.md` | 2026-04-14 | 6.8KB | 製薬業界分析 |
| `output/otsuka_pharma/phase3_usecase_mapping.md` | 2026-04-14 | 10KB | ユースケースマッピング |
| `output/otsuka_pharma/phase4_technology_architecture.md` | 2026-04-14 | 11KB | 技術アーキテクチャ |
| `output/otsuka_pharma/phase5_organization_talent.md` | 2026-04-14 | 8.1KB | 組織・人材戦略 |
| `output/otsuka_pharma/phase6_financial_model.md` | 2026-04-14 | 6.5KB | 財務モデル |
| `output/otsuka_pharma/phase7_roadmap.md` | 2026-04-14 | 11KB | 実行ロードマップ |
| `output/otsuka_pharma/phase8_risk_management.md` | 2026-04-14 | 13KB | リスク管理（GxP対応） |

### 日本化薬（`output/nippon_kayaku/`）

| ファイルパス | 最終更新日 | サイズ | 内容 |
|-------------|-----------|-------|------|
| `output/nippon_kayaku/README.md` | 2026-04-14 | 4.0KB | 目次 |
| `output/nippon_kayaku/full_report.md` | 2026-04-14 | 102KB | **統合レポート** |
| `output/nippon_kayaku/phase1_executive_summary.md` | 2026-04-14 | 8.3KB | エグゼクティブサマリー |
| `output/nippon_kayaku/phase2_industry_analysis.md` | 2026-04-14 | 11KB | 業界分析 |
| `output/nippon_kayaku/phase3_usecase_mapping.md` | 2026-04-14 | 15KB | ユースケースマッピング |
| `output/nippon_kayaku/phase4_technology_architecture.md` | 2026-04-14 | 16KB | 技術アーキテクチャ |
| `output/nippon_kayaku/phase5_organization_talent.md` | 2026-04-14 | 9.8KB | 組織・人材戦略 |
| `output/nippon_kayaku/phase6_financial_model.md` | 2026-04-14 | 9.1KB | 財務モデル |
| `output/nippon_kayaku/phase7_roadmap.md` | 2026-04-14 | 14KB | 実行ロードマップ |
| `output/nippon_kayaku/phase8_risk_management.md` | 2026-04-14 | 20KB | リスク管理 |

### 大樹生命（`output/daiju_life/`）

| ファイルパス | 最終更新日 | サイズ | 内容 |
|-------------|-----------|-------|------|
| `output/daiju_life/README.md` | 2026-04-14 | 2.7KB | 目次 |
| `output/daiju_life/full_report.md` | 2026-04-14 | 100KB | **統合レポート** |
| `output/daiju_life/phase1_executive_summary.md` | 2026-04-14 | 8.4KB | エグゼクティブサマリー |
| `output/daiju_life/phase2_industry_analysis.md` | 2026-04-14 | 11KB | 業界分析 |
| `output/daiju_life/phase3_usecase_mapping.md` | 2026-04-14 | 14KB | ユースケースマッピング |
| `output/daiju_life/phase4_technology_architecture.md` | 2026-04-14 | 14KB | 技術アーキテクチャ |
| `output/daiju_life/phase5_organization_talent.md` | 2026-04-14 | 10KB | 組織・人材戦略 |
| `output/daiju_life/phase6_financial_model.md` | 2026-04-14 | 7.9KB | 財務モデル |
| `output/daiju_life/phase7_roadmap.md` | 2026-04-14 | 13KB | 実行ロードマップ |
| `output/daiju_life/phase8_risk_management.md` | 2026-04-14 | 22KB | リスク管理 |

### ⚠️ 日本製造業（`output/japanese_manufacturing/`） — 旧版（pharma branch）

> このブランチにも `output/japanese_manufacturing/` が存在するが、セキュリティフレームワーク追加前の**旧版**。  
> **最新版**（AIセキュリティ10領域適用済み）は `claude/ai-strategy-generator-hmKWX` ブランチを参照。

---

## バージョン差分まとめ

| 変更内容 | 適用日 | 影響ファイル |
|---------|--------|------------|
| AIセキュリティ10領域フレームワーク追加 | 2026-04-13 | `CLAUDE.md`・`phase4_*`・`phase8_*`（製造業） |
| 統合コマンド `/ai-strategy-full` 追加 | 2026-04-06 | `.claude/skills/ai-strategy-full.md` |
| 経営層PPTXデッキ生成 | 2026-04-05 | `presentation_deck.md`・`*.pptx` |
| CFO/CTO/製造業担当者レビュー生成 | 2026-04-05 | `output/japanese_manufacturing/reviews/` |
| 大塔製薬GxP対応セキュリティ | 2026-04-14 | `output/otsuka_pharma/phase8_*` |
| 日本化薬・大樹生命レポート生成 | 2026-04-14 | `output/nippon_kayaku/`・`output/daiju_life/` |
