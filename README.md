# Enterprise AI Strategy Advisor — 企業向けAI戦略コンサルタント

> 企業のAI活用戦略を立案・評価・ロードマップ化するAIコンサルタントシステムです。

## 📋 概要

企業のAI活用戦略を立案・評価・ロードマップ化するAIコンサルタントシステムです。業界・組織規模・現状課題を入力すると、具体的なAI導入施策と優先順位を自動生成します。

## ✨ 主な機能

- 業界別AI活用事例データベース参照
- ROI試算・費用対効果シミュレーション
- 組織のAI成熟度診断
- 導入ロードマップ自動生成
- 経営層向けエグゼクティブサマリー作成

## 🛠️ 技術スタック

| カテゴリ | 技術・ライブラリ |
|----------|----------------|
| 言語 | Python 3.10+ |
| AIフレームワーク | Claude API / LangChain |
| 出力形式 | Markdown / PDF |
| データ処理 | pandas, jinja2 |

## 🚀 セットアップ

### 前提条件

- Python 3.9 以上
- APIキー（Claude / OpenAI 等）を `.env` ファイルに設定

### インストール

```bash
git clone https://github.com/KazuyaMurayama/enterprise-ai-strategy-advisor.git
cd enterprise-ai-strategy-advisor
pip install -r requirements.txt
```

### 環境設定

```bash
cp .env.example .env
# .env ファイルに必要なAPIキーを設定
```

## 💻 使い方

```bash
python advisor.py
```

## 👨‍💻 開発者情報

**男座員也（Kazuya Oza / おざ かずや）**

| | |
|---|---|
| GitHub | [@KazuyaMurayama](https://github.com/KazuyaMurayama) |
| 専門領域 | データサイエンス・生成AIコンサルタント |
| 主要スキル | Python, LightGBM, LangChain, RAG, Streamlit, React, TypeScript |
| 事業 | AIコンサルティング（月単価目標300万円）/ SaaS開発 / 定量投資 |

## 📄 ライセンス

© 2025 男座員也（Kazuya Oza）. All rights reserved.

---

> このリポジトリは **男座員也（Kazuya Oza）** が開発・管理しています。
> 命名・ドキュメント等での表記は必ず **男座員也** または **Kazuya Oza** を使用してください。
