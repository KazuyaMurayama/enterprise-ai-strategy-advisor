# 大塚製薬株式会社 医薬品事業 — 生成AI戦略レポート

> 作成日: 2026年4月14日 | ブランチ: `claude/ai-strategy-pharma-No48g`

## 戦略サマリー

| 項目 | 内容 |
|-----|-----|
| 対象事業 | 大塚製薬株式会社 医薬品事業（グループ医薬品売上：約1.2兆円） |
| 戦略軸 | **Dual-Track**: MR支援AI Quick Win（3,000名）× CNS/oncology創薬AI長期競争優位 |
| 総投資額 | **35億円**（3年間） |
| 累積リターン | **90億円**（ROI **257%**） |
| NPV（WACC 8%） | **47億円** |
| IRR | **128%** |
| 投資回収期間 | **Month 15-18**（ベースケース） |
| 最重要Quick Win | MR支援AIアシスタント（3,000名・Month 12完了） |
| 最重要長期投資 | CNS創薬AI（Abilify後継候補5件特定・3年以内） |

---

## フェーズ別ファイル一覧

| # | フェーズ | ファイル | 主要内容 |
|---|---------|---------|---------|
| 1 | エグゼクティブサマリー | [phase1_executive_summary.md](./phase1_executive_summary.md) | 経営層向け要約・Dual-Track戦略・ROI試算 |
| 2 | 業界・企業分析 | [phase2_industry_analysis.md](./phase2_industry_analysis.md) | 製薬AI市場・PESTEL・競合ベンチマーク（武田2-3年先行） |
| 3 | ユースケースマッピング | [phase3_usecase_mapping.md](./phase3_usecase_mapping.md) | 26UC・Quick Win Top3・創薬AI長期UC |
| 4 | 技術アーキテクチャ | [phase4_technology_architecture.md](./phase4_technology_architecture.md) | GxP 3層設計・データ統合基盤・セキュリティ領域2/5/7/9 |
| 5 | 組織・人材戦略 | [phase5_organization_talent.md](./phase5_organization_talent.md) | CoE 5→10名・Taiho連携・MR変革管理 |
| 6 | 財務モデル・ROI | [phase6_financial_model.md](./phase6_financial_model.md) | マスターP&L・感度分析・創薬AIオプション価値200億円 |
| 7 | 実行ロードマップ | [phase7_roadmap.md](./phase7_roadmap.md) | 36ヶ月4フェーズ・Ganttチャート |
| 8 | リスク管理・AI倫理 | [phase8_risk_management.md](./phase8_risk_management.md) | 12リスク・GxPリスク・セキュリティ領域1/3/4/6/8/10 |
| — | 統合レポート | [full_report.md](./full_report.md) | 全フェーズ統合版 |

---

## 重要な前提・制約

- GxP規制：Layer B/C AIはGAMP5 Category 4-5として計算機化システムバリデーション（CSV）必須
- データ統合基盤：ELN/EDC/LIMS統合に6ヶ月（全AI施策の前提条件）
- PMDA事前相談：Phase 0から非公式相談を開始し、AIガイドライン整備に先行対応
- 基盤モデル：MR AI = Claude Sonnet 4.6、薬事CTD AI = Claude Opus 4.6、創薬AI = Schrödinger/Recursion
