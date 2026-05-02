# 大樹生命保険株式会社 — 生成AI戦略レポート

> 作成日: 2026年4月13日 | ブランチ: `claude/ai-strategy-pharma-No48g`

## 戦略サマリー

| 項目 | 内容 |
|-----|-----|
| 対象企業 | 大樹生命保険株式会社（旧三井生命、大手生保5-6位） |
| 戦略軸 | **Dual-Track**: 外交員AI Quick Win（15,000名） × 引受AI長期競争優位 |
| 総投資額 | **28億円**（3年間） |
| 累積リターン | **68.5億円**（ROI 245%） |
| NPV（WACC 8%） | **37.5億円** |
| IRR | **118%** |
| 投資回収期間 | **Month 17-19**（ベースケース） |
| 最重要Quick Win | 外交員AIアシスタント全展開（15,000名・Month 12完了） |

---

## フェーズ別ファイル一覧

| # | フェーズ | ファイル | 主要内容 |
|---|---------|---------|---------|
| 1 | エグゼクティブサマリー | [phase1_executive_summary.md](./phase1_executive_summary.md) | 経営層向け1枚要約・Dual-Track戦略・ROI試算 |
| 2 | 業界・企業分析 | [phase2_industry_analysis.md](./phase2_industry_analysis.md) | 生命保険市場40兆円・PESTEL・競合ベンチマーク |
| 3 | ユースケースマッピング | [phase3_usecase_mapping.md](./phase3_usecase_mapping.md) | 27UC・プライオリティマトリクス・Top10 |
| 4 | 技術アーキテクチャ | [phase4_technology_architecture.md](./phase4_technology_architecture.md) | 3層設計・勘定系APIブリッジ・セキュリティ領域2/5/7/9 |
| 5 | 組織・人材戦略 | [phase5_organization_talent.md](./phase5_organization_talent.md) | CoE 6→15名・外交員変革管理・アクチュアリーAI |
| 6 | 財務モデル・ROI | [phase6_financial_model.md](./phase6_financial_model.md) | マスターP&L・感度分析・投資ステージゲート |
| 7 | 実行ロードマップ | [phase7_roadmap.md](./phase7_roadmap.md) | 36ヶ月4フェーズ・Ganttチャート・経営報告タイミング |
| 8 | リスク管理・AI倫理 | [phase8_risk_management.md](./phase8_risk_management.md) | 12リスク・AIガバナンス・セキュリティ領域1/3/4/6/8/10 |
| — | 統合レポート | [full_report.md](./full_report.md) | 全フェーズ統合版（1,500行超） |

---

## 重要な前提・制約

- 金融庁規制：引受AI・支払審査AIはPhase 0からの事前相談が必須
- 勘定系APIブリッジ：COBOL/メインフレーム連携に6-9ヶ月（全AIの前提条件）
- 外交員受容：15,000名の変革管理が最大ROI変数（利用率±20%でROI±35%変動）
- 基盤モデル：外交員AI = Claude Sonnet 4.6（日本語最適）、引受AIレポート = Claude Opus 4.6
