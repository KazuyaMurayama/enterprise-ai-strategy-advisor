# FILE_INDEX — enterprise-ai-strategy-advisor

> ⚠️ このファイルは自動生成です。手動編集は次回更新で上書きされます。

| 項目 | 値 |
|---|---|
| リポジトリ | KazuyaMurayama/enterprise-ai-strategy-advisor |
| ブランチ | main |
| 総ファイル数 | 118 |
| 最終更新 | 2026-05-02 |
| 管理者 | 男座員也（Kazuya Oza） |

---

## カテゴリ別サマリー

| カテゴリ | ファイル数 |
|---|---|
| Documentation | 115 |
| Asset | 1 |
| Config | 1 |
| Other | 1 |

---

## ディレクトリ構成

```
.
├── .claude/
│   └── skills/
│       ├── ai-strategy_20260405.md
│       ├── ai-strategy-full_20260406.md
│       ├── ai-strategy-full.md
│       ├── ai-strategy.md
│       ├── executive-summary_20260405.md
│       ├── executive-summary.md
│       ├── industry-analysis_20260405.md
│       ├── industry-analysis.md
│       ├── roi-calculator_20260405.md
│       ├── roi-calculator.md
│       ├── usecase-mapper_20260405.md
│       └── usecase-mapper.md
├── output/
│   ├── amazon_japan/
│   │   ├── full_report.md
│   │   ├── phase1_executive_summary.md
│   │   ├── phase2_industry_analysis.md
│   │   ├── phase3_usecase_mapping.md
│   │   ├── phase4_technology_architecture.md
│   │   ├── phase5_organization_talent.md
│   │   ├── phase6_financial_model.md
│   │   ├── phase7_roadmap.md
│   │   ├── phase8_risk_management.md
│   │   └── README.md
│   ├── cross_company_usecase_matrix/
│   │   └── ai_usecase_proposals.md
│   ├── daiju_life/
│   │   ├── full_report.md
│   │   ├── phase1_executive_summary.md
│   │   ├── phase2_industry_analysis.md
│   │   ├── phase3_usecase_mapping.md
│   │   ├── phase4_technology_architecture.md
│   │   ├── phase5_organization_talent.md
│   │   ├── phase6_financial_model.md
│   │   ├── phase7_roadmap.md
│   │   ├── phase8_risk_management.md
│   │   └── README.md
│   ├── daishi_hokuetsu/
│   │   ├── full_report.md
│   │   ├── phase1_executive_summary.md
│   │   ├── phase2_industry_analysis.md
│   │   ├── phase3_usecase_mapping.md
│   │   ├── phase4_technology_architecture.md
│   │   ├── phase5_organization_talent.md
│   │   ├── phase6_financial_model.md
│   │   ├── phase7_roadmap.md
│   │   ├── phase8_risk_management.md
│   │   └── README.md
│   ├── ebara/
│   │   ├── full_report.md
│   │   ├── phase1_executive_summary.md
│   │   ├── phase2_industry_analysis.md
│   │   ├── phase3_usecase_mapping.md
│   │   ├── phase4_technology_architecture.md
│   │   ├── phase5_organization_talent.md
│   │   ├── phase6_financial_model.md
│   │   ├── phase7_roadmap.md
│   │   ├── phase8_risk_management.md
│   │   └── README.md
│   ├── japanese_manufacturing/
│   │   ├── reviews/
│   │   │   ... (3 items)
│   │   ├── ai_strategy_presentation.pptx
│   │   ├── full_report.md
│   │   ├── phase1_executive_summary.md
│   │   ├── phase2_industry_analysis.md
│   │   ├── phase3_usecase_mapping.md
│   │   ├── phase4_technology_architecture.md
│   │   ├── phase5_organization_talent.md
│   │   ├── phase6_financial_model.md
│   │   ├── phase7_roadmap.md
│   │   ├── phase8_risk_management.md
│   │   ├── presentation_deck.md
│   │   └── README.md
│   ├── nippon_kayaku/
│   │   ├── full_report.md
│   │   ├── phase1_executive_summary.md
│   │   ├── phase2_industry_analysis.md
│   │   ├── phase3_usecase_mapping.md
│   │   ├── phase4_technology_architecture.md
│   │   ├── phase5_organization_talent.md
│   │   ├── phase6_financial_model.md
│   │   ├── phase7_roadmap.md
│   │   ├── phase8_risk_management.md
│   │   └── README.md
│   ├── otsuka_pharma/
│   │   ├── full_report.md
│   │   ├── phase1_executive_summary.md
│   │   ├── phase2_industry_analysis.md
│   │   ├── phase3_usecase_mapping.md
│   │   ├── phase4_technology_architecture.md
│   │   ├── phase5_organization_talent.md
│   │   ├── phase6_financial_model.md
│   │   ├── phase7_roadmap.md
│   │   ├── phase8_risk_management.md
│   │   └── README.md
│   ├── shikoku_electric/
│   │   ├── full_report.md
│   │   ├── phase1_executive_summary.md
│   │   ├── phase2_industry_analysis.md
│   │   ├── phase3_usecase_mapping.md
│   │   ├── phase4_technology_architecture.md
│   │   ├── phase5_organization_talent.md
│   │   ├── phase6_financial_model.md
│   │   ├── phase7_roadmap.md
│   │   ├── phase8_risk_management.md
│   │   └── README.md
│   ├── 太陽油脂_SCM_BPR/
│   │   ├── appendix_hearing_log.md
│   │   ├── board_memo_0520.md
│   │   ├── full_report.md
│   │   ├── phase1_executive_summary.md
│   │   ├── phase2_as_is_analysis.md
│   │   ├── phase3_judgment_work_framework.md
│   │   ├── phase4_ai_rpa_mapping.md
│   │   ├── phase5_headcount_simulation.md
│   │   ├── phase6_roadmap_stakeholder.md
│   │   ├── phase7_risk_governance.md
│   │   └── README.md
│   └── .gitkeep
├── templates/
│   ├── report-template_20260405.md
│   └── report-template.md
├── .gitignore
├── CLAUDE.md
├── FILE_INDEX.md
├── README.md
├── tasks.md
└── Timeout_Prevention.md
```

---

## ファイル詳細

### Documentation (115件)

<details>
<summary>クリックして展開 (115件)</summary>

| ファイル | サイズ | 説明 |
|---|---|---|
| `.claude/skills/ai-strategy_20260405.md` | 2.9 KB | Claude Code 設定・スキル |
| `.claude/skills/ai-strategy-full_20260406.md` | 6.6 KB | Claude Code 設定・スキル |
| `.claude/skills/ai-strategy-full.md` | 8.8 KB | Claude Code 設定・スキル |
| `.claude/skills/ai-strategy.md` | 2.8 KB | Claude Code 設定・スキル |
| `.claude/skills/executive-summary_20260405.md` | 1.5 KB | Claude Code 設定・スキル |
| `.claude/skills/executive-summary.md` | 1.4 KB | Claude Code 設定・スキル |
| `.claude/skills/industry-analysis_20260405.md` | 1.9 KB | Claude Code 設定・スキル |
| `.claude/skills/industry-analysis.md` | 1.8 KB | Claude Code 設定・スキル |
| `.claude/skills/roi-calculator_20260405.md` | 2.0 KB | Claude Code 設定・スキル |
| `.claude/skills/roi-calculator.md` | 1.9 KB | Claude Code 設定・スキル |
| `.claude/skills/usecase-mapper_20260405.md` | 1.7 KB | Claude Code 設定・スキル |
| `.claude/skills/usecase-mapper.md` | 1.6 KB | Claude Code 設定・スキル |
| `CLAUDE.md` | 8.0 KB | Claude Code プロジェクト設定・命名ルール |
| `FILE_INDEX.md` | 10.2 KB | （このファイル）全ファイルインデックス |
| `output/amazon_japan/full_report.md` | 77.0 KB | リサーチ出力データ |
| `output/amazon_japan/phase1_executive_summary.md` | 6.2 KB | リサーチ出力データ |
| `output/amazon_japan/phase2_industry_analysis.md` | 11.5 KB | リサーチ出力データ |
| `output/amazon_japan/phase3_usecase_mapping.md` | 10.6 KB | リサーチ出力データ |
| `output/amazon_japan/phase4_technology_architecture.md` | 12.3 KB | リサーチ出力データ |
| `output/amazon_japan/phase5_organization_talent.md` | 8.8 KB | リサーチ出力データ |
| `output/amazon_japan/phase6_financial_model.md` | 6.1 KB | リサーチ出力データ |
| `output/amazon_japan/phase7_roadmap.md` | 9.7 KB | リサーチ出力データ |
| `output/amazon_japan/phase8_risk_management.md` | 11.9 KB | リサーチ出力データ |
| `output/amazon_japan/README.md` | 2.5 KB | リポジトリ概要・セットアップ手順 |
| `output/cross_company_usecase_matrix/ai_usecase_proposals.md` | 53.7 KB | リサーチ出力データ |
| `output/daiju_life/full_report.md` | 97.8 KB | リサーチ出力データ |
| `output/daiju_life/phase1_executive_summary.md` | 8.3 KB | リサーチ出力データ |
| `output/daiju_life/phase2_industry_analysis.md` | 10.4 KB | リサーチ出力データ |
| `output/daiju_life/phase3_usecase_mapping.md` | 13.8 KB | リサーチ出力データ |
| `output/daiju_life/phase4_technology_architecture.md` | 13.3 KB | リサーチ出力データ |
| `output/daiju_life/phase5_organization_talent.md` | 10.0 KB | リサーチ出力データ |
| `output/daiju_life/phase6_financial_model.md` | 7.7 KB | リサーチ出力データ |
| `output/daiju_life/phase7_roadmap.md` | 12.4 KB | リサーチ出力データ |
| `output/daiju_life/phase8_risk_management.md` | 22.0 KB | リサーチ出力データ |
| `output/daiju_life/README.md` | 2.6 KB | リポジトリ概要・セットアップ手順 |
| `output/daishi_hokuetsu/full_report.md` | 58.9 KB | リサーチ出力データ |
| `output/daishi_hokuetsu/phase1_executive_summary.md` | 4.7 KB | リサーチ出力データ |
| `output/daishi_hokuetsu/phase2_industry_analysis.md` | 8.4 KB | リサーチ出力データ |
| `output/daishi_hokuetsu/phase3_usecase_mapping.md` | 8.3 KB | リサーチ出力データ |
| `output/daishi_hokuetsu/phase4_technology_architecture.md` | 7.6 KB | リサーチ出力データ |
| `output/daishi_hokuetsu/phase5_organization_talent.md` | 6.3 KB | リサーチ出力データ |
| `output/daishi_hokuetsu/phase6_financial_model.md` | 4.1 KB | リサーチ出力データ |
| `output/daishi_hokuetsu/phase7_roadmap.md` | 9.0 KB | リサーチ出力データ |
| `output/daishi_hokuetsu/phase8_risk_management.md` | 10.4 KB | リサーチ出力データ |
| `output/daishi_hokuetsu/README.md` | 2.1 KB | リポジトリ概要・セットアップ手順 |
| `output/ebara/full_report.md` | 68.8 KB | リサーチ出力データ |
| `output/ebara/phase1_executive_summary.md` | 5.0 KB | リサーチ出力データ |
| `output/ebara/phase2_industry_analysis.md` | 8.9 KB | リサーチ出力データ |
| `output/ebara/phase3_usecase_mapping.md` | 7.0 KB | リサーチ出力データ |
| `output/ebara/phase4_technology_architecture.md` | 13.0 KB | リサーチ出力データ |
| `output/ebara/phase5_organization_talent.md` | 7.9 KB | リサーチ出力データ |
| `output/ebara/phase6_financial_model.md` | 7.2 KB | リサーチ出力データ |
| `output/ebara/phase7_roadmap.md` | 8.9 KB | リサーチ出力データ |
| `output/ebara/phase8_risk_management.md` | 11.0 KB | リサーチ出力データ |
| `output/ebara/README.md` | 2.4 KB | リポジトリ概要・セットアップ手順 |
| `output/japanese_manufacturing/full_report.md` | 158.1 KB | リサーチ出力データ |
| `output/japanese_manufacturing/phase1_executive_summary.md` | 8.8 KB | リサーチ出力データ |
| `output/japanese_manufacturing/phase2_industry_analysis.md` | 20.6 KB | リサーチ出力データ |
| `output/japanese_manufacturing/phase3_usecase_mapping.md` | 24.6 KB | リサーチ出力データ |
| `output/japanese_manufacturing/phase4_technology_architecture.md` | 23.6 KB | リサーチ出力データ |
| `output/japanese_manufacturing/phase5_organization_talent.md` | 18.7 KB | リサーチ出力データ |
| `output/japanese_manufacturing/phase6_financial_model.md` | 22.1 KB | リサーチ出力データ |
| `output/japanese_manufacturing/phase7_roadmap.md` | 22.1 KB | リサーチ出力データ |
| `output/japanese_manufacturing/phase8_risk_management.md` | 27.8 KB | リサーチ出力データ |
| `output/japanese_manufacturing/presentation_deck.md` | 23.4 KB | リサーチ出力データ |
| `output/japanese_manufacturing/README.md` | 4.6 KB | リポジトリ概要・セットアップ手順 |
| `output/japanese_manufacturing/reviews/client_a_cfo.md` | 4.5 KB | リサーチ出力データ |
| `output/japanese_manufacturing/reviews/client_b_cto.md` | 5.6 KB | リサーチ出力データ |
| `output/japanese_manufacturing/reviews/client_c_manufacturing.md` | 5.7 KB | リサーチ出力データ |
| `output/nippon_kayaku/full_report.md` | 100.1 KB | リサーチ出力データ |
| `output/nippon_kayaku/phase1_executive_summary.md` | 8.1 KB | リサーチ出力データ |
| `output/nippon_kayaku/phase2_industry_analysis.md` | 10.3 KB | リサーチ出力データ |
| `output/nippon_kayaku/phase3_usecase_mapping.md` | 14.3 KB | リサーチ出力データ |
| `output/nippon_kayaku/phase4_technology_architecture.md` | 15.4 KB | リサーチ出力データ |
| `output/nippon_kayaku/phase5_organization_talent.md` | 9.6 KB | リサーチ出力データ |
| `output/nippon_kayaku/phase6_financial_model.md` | 8.9 KB | リサーチ出力データ |
| `output/nippon_kayaku/phase7_roadmap.md` | 13.5 KB | リサーチ出力データ |
| `output/nippon_kayaku/phase8_risk_management.md` | 20.0 KB | リサーチ出力データ |
| `output/nippon_kayaku/README.md` | 3.9 KB | リポジトリ概要・セットアップ手順 |
| `output/otsuka_pharma/full_report.md` | 70.2 KB | リサーチ出力データ |
| `output/otsuka_pharma/phase1_executive_summary.md` | 5.4 KB | リサーチ出力データ |
| `output/otsuka_pharma/phase2_industry_analysis.md` | 6.7 KB | リサーチ出力データ |
| `output/otsuka_pharma/phase3_usecase_mapping.md` | 9.9 KB | リサーチ出力データ |
| `output/otsuka_pharma/phase4_technology_architecture.md` | 10.8 KB | リサーチ出力データ |
| `output/otsuka_pharma/phase5_organization_talent.md` | 7.9 KB | リサーチ出力データ |
| `output/otsuka_pharma/phase6_financial_model.md` | 6.4 KB | リサーチ出力データ |
| `output/otsuka_pharma/phase7_roadmap.md` | 10.3 KB | リサーチ出力データ |
| `output/otsuka_pharma/phase8_risk_management.md` | 12.7 KB | リサーチ出力データ |
| `output/otsuka_pharma/README.md` | 2.7 KB | リポジトリ概要・セットアップ手順 |
| `output/shikoku_electric/full_report.md` | 54.8 KB | リサーチ出力データ |
| `output/shikoku_electric/phase1_executive_summary.md` | 4.8 KB | リサーチ出力データ |
| `output/shikoku_electric/phase2_industry_analysis.md` | 8.8 KB | リサーチ出力データ |
| `output/shikoku_electric/phase3_usecase_mapping.md` | 7.9 KB | リサーチ出力データ |
| `output/shikoku_electric/phase4_technology_architecture.md` | 7.1 KB | リサーチ出力データ |
| `output/shikoku_electric/phase5_organization_talent.md` | 6.0 KB | リサーチ出力データ |
| `output/shikoku_electric/phase6_financial_model.md` | 3.8 KB | リサーチ出力データ |
| `output/shikoku_electric/phase7_roadmap.md` | 7.3 KB | リサーチ出力データ |
| `output/shikoku_electric/phase8_risk_management.md` | 9.2 KB | リサーチ出力データ |
| `output/shikoku_electric/README.md` | 2.2 KB | リポジトリ概要・セットアップ手順 |
| `output/太陽油脂_SCM_BPR/appendix_hearing_log.md` | 8.5 KB | リサーチ出力データ |
| `output/太陽油脂_SCM_BPR/board_memo_0520.md` | 6.9 KB | リサーチ出力データ |
| `output/太陽油脂_SCM_BPR/full_report.md` | 95.7 KB | リサーチ出力データ |
| `output/太陽油脂_SCM_BPR/phase1_executive_summary.md` | 7.3 KB | リサーチ出力データ |
| `output/太陽油脂_SCM_BPR/phase2_as_is_analysis.md` | 12.9 KB | リサーチ出力データ |
| `output/太陽油脂_SCM_BPR/phase3_judgment_work_framework.md` | 21.0 KB | リサーチ出力データ |
| `output/太陽油脂_SCM_BPR/phase4_ai_rpa_mapping.md` | 10.2 KB | リサーチ出力データ |
| `output/太陽油脂_SCM_BPR/phase5_headcount_simulation.md` | 11.8 KB | リサーチ出力データ |
| `output/太陽油脂_SCM_BPR/phase6_roadmap_stakeholder.md` | 8.1 KB | リサーチ出力データ |
| `output/太陽油脂_SCM_BPR/phase7_risk_governance.md` | 9.0 KB | リサーチ出力データ |
| `output/太陽油脂_SCM_BPR/README.md` | 5.3 KB | リポジトリ概要・セットアップ手順 |
| `README.md` | 2.1 KB | リポジトリ概要・セットアップ手順 |
| `tasks.md` | 1.2 KB | タスク管理・セッション履歴 |
| `templates/report-template_20260405.md` | 6.6 KB | Markdown ドキュメント |
| `templates/report-template.md` | 6.5 KB | Markdown ドキュメント |
| `Timeout_Prevention.md` | 4.9 KB | タイムアウト対策ガイド |

</details>

### Asset (1件)

| ファイル | サイズ | 説明 |
|---|---|---|
| `output/japanese_manufacturing/ai_strategy_presentation.pptx` | 65.4 KB | リサーチ出力データ |

### Config (1件)

| ファイル | サイズ | 説明 |
|---|---|---|
| `.gitignore` | 377 B | Git 除外設定 |

### Other (1件)

| ファイル | サイズ | 説明 |
|---|---|---|
| `output/.gitkeep` | - | ファイル |

---

_自動生成: 2026-05-02 | 管理者: 男座員也（Kazuya Oza）_
