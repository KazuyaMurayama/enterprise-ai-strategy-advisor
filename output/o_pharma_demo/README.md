# O製薬 医薬品事業 — 生成AI戦略レポート（デモ用匿名版）

> 作成日: 2026年4月14日 | ブランチ: `main`

> **本レポートはデモンストレーション用にマスク処理した匿名版です。**
>
> | コード | 種別 |
> |---|---|
> | **O製薬** | 自社（国内大手製薬・CNS領域に強み） |
> | **OT製薬** | 自社グループのがん領域子会社 |
> | **OF食品** | 自社グループのOTC・食品子会社 |
> | **T製薬 / A製薬 / D製薬 / C製薬 / E製薬** | 国内競合製薬5社 |
> | **主力CNS製品X** | 自社主力CNS製品（長期実績品） |
> | **競合ADC薬A / 競合オレキシン薬B / 競合抗アミロイド薬C** | 競合パイプライン代表例 |
> | **競合AI創薬子会社α** | 競合のAI創薬子会社 |
> | **P1〜P7** | 外部技術パートナー（RWD/ゲノム診断/計算化学/画像創薬/生成創薬/CRO/SaaS） |
> | 数値 | 規模感を保ちつつ±15〜20%の範囲で丸め済み |

---

## 戦略サマリー

| 項目 | 内容 |
|-----|-----|
| 対象事業 | O製薬 医薬品事業（グループ医薬品売上：1兆円超規模） |
| 戦略軸 | **Dual-Track**: MR支援AI Quick Win（約3,000名）× CNS/oncology創薬AI長期競争優位 |
| 総投資額 | **約30億円**（3年間） |
| 累積リターン | **約80億円**（ROI **約250%**） |
| NPV（WACC 8%） | **約45億円** |
| IRR | **約130%** |
| 投資回収期間 | **Month 15〜18**（ベースケース） |
| 最重要Quick Win | MR支援AIアシスタント（約3,000名・Month 12完了） |
| 最重要長期投資 | CNS創薬AI（主力CNS製品X後継候補5件特定・3年以内） |

---

## フェーズ別ファイル一覧

| # | フェーズ | ファイル | 主要内容 |
|---|---------|---------|---------|
| 1 | エグゼクティブサマリー | [phase1_executive_summary.md](./phase1_executive_summary.md) | 経営層向け要約・Dual-Track戦略・ROI試算 |
| 2 | 業界・企業分析 | [phase2_industry_analysis.md](./phase2_industry_analysis.md) | 製薬AI市場・PESTEL・競合ベンチマーク |
| 3 | ユースケースマッピング | [phase3_usecase_mapping.md](./phase3_usecase_mapping.md) | 26UC・Quick Win Top3・創薬AI長期UC |
| 4 | 技術アーキテクチャ | [phase4_technology_architecture.md](./phase4_technology_architecture.md) | GxP 3層設計・データ統合基盤・セキュリティ |
| 5 | 組織・人材戦略 | [phase5_organization_talent.md](./phase5_organization_talent.md) | CoE 5→10名・OT製薬連携・MR変革管理 |
| 6 | 財務モデル・ROI | [phase6_financial_model.md](./phase6_financial_model.md) | マスターP&L・感度分析・創薬AIオプション価値 |
| 7 | 実行ロードマップ | [phase7_roadmap.md](./phase7_roadmap.md) | 36ヶ月4フェーズ・Ganttチャート |
| 8 | リスク管理・AI倫理 | [phase8_risk_management.md](./phase8_risk_management.md) | 12リスク・GxPリスク・セキュリティ |
| — | 統合レポート | [full_report.md](./full_report.md) | 全フェーズ統合版 |

---

## 重要な前提・制約

- GxP規制：Layer B/C AIはGAMP5 Category 4-5として計算機化システムバリデーション（CSV）必須
- データ統合基盤：ELN/EDC/LIMS統合に6ヶ月（全AI施策の前提条件）
- PMDA事前相談：Phase 0から非公式相談を開始し、AIガイドライン整備に先行対応
- 基盤モデル：MR AI = Claude Sonnet 4.6、薬事CTD AI = Claude Opus 4.6、創薬AI = 計算化学SaaSベンダーP3/画像創薬AIベンダーP4
