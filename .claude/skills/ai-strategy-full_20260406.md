<!-- ファイル情報: ai-strategy-full.md | 最終更新: 2026-04-06 | 版管理コピー -->
---
name: ai-strategy-full
description: 企業名/業界名を入力するだけで、MBB水準AI戦略レポート→品質改善→PPTXまで一気通貫で自動生成する統合コマンド
user_invocable: true
---

# AI戦略レポート 一気通貫自動生成（Full Pipeline）

企業名/業界名1つから、以下の全工程を自動で実行する統合コマンド。

```
/ai-strategy-full トヨタ自動車
/ai-strategy-full 日本の金融業界
/ai-strategy-full 小売業 --skip-pptx
```

## 引数

`$ARGUMENTS` から以下を解析:
- **必須**: 企業名 or 業界名（第1引数）
- **オプション**:
  - `--skip-review`: クライアントレビュー＋改善をスキップ
  - `--skip-pptx`: PPTX生成をスキップ
  - `--scale <small|medium|large>`: 対象企業規模（default: medium = 売上1,000億/5,000名）
  - `--lang <ja|en>`: 出力言語（default: ja）

---

## 全体パイプライン（4ステージ）

```
Stage 1        Stage 2         Stage 3          Stage 4
レポート生成 → 品質改善      → クライアント   → プレゼン生成
(8フェーズ)    (数値整合+     レビュー＋       (MD+PPTX
               フレームワーク  MBB改善          20枚)
               強化)
```

### タイムアウト対策（必須ルール）
- **1フェーズ = 1ファイル保存**。複数フェーズをまとめない
- **2フェーズごとにgit commit**。ロールバック可能に
- **Stage完了ごとにgit push**

---

## Stage 1: レポート生成（8フェーズ）

対象を `{target}` とする（引数から取得）。
出力先: `output/{target_slug}/`（日本語はスネークケースに変換）

### 実行順序

各フェーズを**1つずつ順番に**実行し、完了後即座にファイル保存:

| Step | ファイル | 内容 | 必須要素 |
|:----:|---------|------|---------|
| 1 | `phase2_industry_analysis.md` | PESTEL+AI変数、Porter's 5 Forces+AI変数、競合ベンチマーク3-5社、AI成熟度評価 | 数値付き市場規模、導入率 |
| 2 | `phase3_usecase_mapping.md` | バリューチェーン分析、2×2プライオリティマトリクス、Top10ユースケース詳細 | 各UCに投資額・効果額・回収期間 |
| 3 | `phase4_technology_architecture.md` | Build/Buy/Partner判定表、基盤モデル選定（5軸評価）、データ戦略5段階、**AIセキュリティアーキテクチャ**（Zero Trust/サプライチェーン/PETs/データリネージ） | TCO比較、マルチモデル戦略、セキュリティ投資 |
| 4 | `phase5_organization_talent.md` | CoE設計（ハイブリッド型）、人材マトリクス、チェンジマネジメント（90日計画） | 人数・コスト付き |
| 5 | `phase6_financial_model.md` | **★マスターP&L**（Single Source of Truth）。投資計画、リターン試算、感度分析3シナリオ、NPV/IRR | 段階的発現率、隠れコスト明示、会計処理方針 |
| 6 | `phase7_roadmap.md` | 5フェーズロードマップ、稟議プロセス（日本企業の場合）、Go/No-Go基準、撤退基準 | 月次タイムライン、ステージゲート |
| 7 | `phase8_risk_management.md` | リスク一覧（6カテゴリ）、AI倫理ガバナンス、ハルシネーション対策3層防御、**先進AIセキュリティ10領域** | EU AI Act分類、CLAUDE.mdの10領域セキュリティフレームワーク準拠 |
| 8 | `phase1_executive_summary.md` | **Phase6の数値を引用**して作成。3投資オプション、KPIサマリー、用語集 | Phase6と完全整合 |

> **注**: Phase1はPhase6完成後に作成する（数値の整合性確保のため）

### 各フェーズの必須ルール
- 冒頭に「このセクションの要点」3行
- すべての提言に `[推奨]` タグと理由
- 数値のない提言は禁止（フェルミ推定可）
- 表・マトリクス・フレームワークを多用
- 末尾に `> **So What?**` で経営的含意
- MECE構造化を徹底

### Phase 6（マスターP&L）の必須構成
1. 基本前提条件テーブル（企業規模、割引率、発現率）
2. **段階的効果発現率**（Y1=40%/Y2=60%/Y3=80%推奨）
3. 年度別投資内訳（技術/人材/組織/隠れコスト）
4. **隠れコストの明示計上**（既存システム改修、データクレンジング、セキュリティ）
5. リターン試算（Raw→発現率適用後）
6. P&L統合表（ベースケース）
7. 感度分析（3シナリオ＋変数別感度テーブル）
8. NPV/IRR分析
9. 3投資オプション（フル/段階/最小限）
10. 会計処理方針（CAPEX/OPEX区分）
11. 投資判断サマリー

### Stage 1完了時の成果物
- `phase1_executive_summary.md` 〜 `phase8_risk_management.md`（8ファイル）
- `README.md`（目次＋KPIサマリー）
- `full_report.md`（全フェーズ統合）
- git commit + push

---

## Stage 2: 品質改善

### 数値整合性チェック
Phase 6の主要数値（総投資額、ROI、回収期間、NPV）が全フェーズで統一されているか確認。不整合があれば修正。

### フレームワーク強化チェックリスト
- [ ] PESTEL交差影響分析（Phase 2）
- [ ] BCGアンビション・マトリクス（Phase 3）
- [ ] MLOps運用体制（Phase 4）
- [ ] 労組対応（Phase 5、日本企業の場合）
- [ ] 撤退基準・投資縮小シナリオ（Phase 7）

### Stage 2完了時: git commit + push

---

## Stage 3: クライアントレビュー＋MBB改善（`--skip-review`でスキップ可）

### クライアントエージェント3体
| # | 視点 | 評価軸 |
|---|------|--------|
| 1 | **財務** CFO | ROI前提の現実性、会計処理、撤退基準 |
| 2 | **技術** CTO | 技術実現可能性、セキュリティ |
| 3 | **現場** 事業部門長 | 導入実行性、チェンジマネジメント |

各クライアントのレビューを `output/{target_slug}/reviews/` に保存。
MBBパートナーエージェントが改善を実施し、git commit + push。

---

## Stage 4: プレゼンテーション生成（`--skip-pptx`でスキップ可）

### Markdownスライド（20枚・3幕構成）
- 第1幕（1-3）: 結論ファースト
- 第2幕（4-14）: インサイト
- 第3幕（15-20）: リスク・Next Steps・Q&A

### PPTX生成
- python-pptxで生成: 16:9、ダークネイビーテーマ
- `output/{target_slug}/ai_strategy_presentation.pptx`

### Stage 4完了時: git commit + push

---

## 完了報告
生成された全ファイルのGitHubハイパーリンク一覧（表形式）と主要KPIを報告。
