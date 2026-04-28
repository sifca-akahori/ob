---
date: 2026-04-25
category: 研究
source: Google DeepMind Blog
url: https://blog.google/innovation-and-ai/models-and-research/gemini-models/next-generation-gemini-deep-research/
impact: 2
tags: [AI, 研究, Google, Gemini, DeepResearch, MCP, BrowseComp, エージェント]
cssclasses:
  - hide-properties
  - ai-news
---

# 🔬 Google「Deep Research Max」発表——BrowseComp 85.9、MCP対応で社内DBにも潜る

> [!tip] TL;DR
> GoogleがGemini 3.1 Pro搭載の **Deep Research Max** を発表。BrowseCompベンチマークで **85.9点**（Gemini 3 Pro比 **+25点超**）を達成し、**MCPサポート**で外部ツール・社内DBへのアクセスと、ネイティブ図表・インフォグラフィック生成を標準装備。長時間自律リサーチエージェントとしてPerplexityやOpenAI Deep Researchと正面衝突する。

> [!info] 引用元
> - 🔗 **URL**: [Google DeepMind Blog](https://blog.google/innovation-and-ai/models-and-research/gemini-models/next-generation-gemini-deep-research/)
> - 📅 **公開日**: 2026-04-22（週内継続評価中）
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> GoogleはGemini API向けにDeep ResearchとDeep Research Maxの2バリアントを刷新・公開した。Gemini 3.1 Proを基盤とするMaxバージョンはBrowseCompで **85.9点** を記録し、前世代のGemini 3 Pro（60点台）から大幅に向上。特筆すべきは **MCP（Model Context Protocol）サポートの標準実装**で、企業の社内システムへのリアルタイムアクセスが可能になった。High-quality charts/infographicsのインライン生成、非同期バックグラウンド実行、レイテンシ重視のResearchとコスト重視のMax Pro-Maxという2バリアント設計で用途に応じた使い分けを訴求する。

---

## 📊 詳細レポート

![[2026-04-25_Google-Deep-Research-Max.svg|1600]]

---

## 🔍 特記事項

> [!note] BrowseComp 85.9の意味——どんな能力を測るベンチマークか
> BrowseCompはOpenAIが提案した「複数ステップのウェブブラウジングを要する難問」を解く能力を測るベンチマーク。「特定の論文の著者が2018年に共同研究した大学を特定せよ」といった、単一検索では解けない問題群で構成される。85.9はOpenAI o3-class（約75〜80点台）やPerplexity Pro（60点台）を上回るスコアとされており、「長時間・多ステップ調査タスク」でGoogleが一歩抜け出した可能性を示唆する。ただしBrowseComp自体の問題セットの更新頻度とリーク可能性には注意が必要。

> [!note] MCPとの統合が意味すること——エンタープライズ展開の要
> 2026年4月にMCPが月間97Mインストールを突破し業界標準化が進む中、Deep ResearchへのMCP統合は「公共Webだけでなく企業内部ナレッジを包含した調査エージェント」を可能にする。例えば、ConfluenceのナレッジベースとSlackのスレッドとGoogle DriveのExcelシートを横断検索し、最終レポートをインライン図表付きで出力するワークフローが自然言語指示だけで構築できる。これはコンサルティング・リサーチ・Legal Discoveryといった高単価知識労働の自動化に直結する。

> [!note] PerplexityとOpenAI Deep Researchとの三つ巴競争
> Deep Research Maxの発表でGoogleはPerplexityのPro Search（約60点台）とOpenAI Deep Research（ChatGPT Pro提供中、70〜80点台推計）との直接競合に踏み込んだ。Googleの優位点はGemini APIの低コストとGCP企業インフラとの統合容易性。対してOpenAIはCodex連携による「調査→コード実装→テスト」の一貫パイプライン、PerplexityはUX洗練と引用精度で差別化を試みる。この三つ巴は2026年後半にかけてさらに激化する見通し。

> [!note] Gemini 3.1 Proの位置づけ——Deep Researchに特化した強化
> Gemini 3.1 Proは全般的フラッグシップというよりも「長時間・多ステップ・情報統合タスク」に特化したトレーニングが施された可能性が高い。実際BrowseComp以外のベンチ（コーディング・数学）での優位性は示されておらず、GoogleはモデルをコアLLMとしてではなくエージェント特化パッケージとして売り出している。これはOpenAIのo3（推論特化）、Anthropicのモデルファミリー戦略と異なるアプローチで、「ユースケース別モデル特化」トレンドを先取りしている。

---

## 🔗 関連記事

- [[2026-04-22_Google-Cloud-Next-Gemini-Enterprise]]
- [[2026-04-23_MCP-97M-Infrastructure-Standard]]
- [[2026-W17|📅 Week 17 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
