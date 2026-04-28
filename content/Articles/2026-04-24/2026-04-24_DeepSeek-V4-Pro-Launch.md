---
date: 2026-04-24
category: 研究
source: Bloomberg / DeepSeek Technical Report
url: https://www.bloomberg.com/news/articles/2026-04-24/deepseek-unveils-newest-flagship-a-year-after-ai-breakthrough
impact: 3
tags: [AI, DeepSeek, LLM, オープンソース, ベンチマーク, 中国AI, コーディング]
cssclasses:
  - hide-properties
  - ai-news
---

# 🐋 DeepSeek V4 Pro/Flash 公開——1.6兆パラメータ・$3.48で米勢に対抗

> [!tip] TL;DR
> DeepSeekがV3の後継「V4 Pro／Flash」をプレビュー公開。**1.6兆総パラメータ・49B活性・1Mトークンコンテキスト**、SWE-bench 80.6%で最上位クラスに到達。出力単価はOpenAIの **1/9（$3.48 vs $30）** という価格破壊で、クローズドソースの経済合理性を直撃する。

> [!info] 引用元
> - 🔗 **URL**: [Bloomberg](https://www.bloomberg.com/news/articles/2026-04-24/deepseek-unveils-newest-flagship-a-year-after-ai-breakthrough)
> - 📅 **公開日**: 2026-04-24
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐⭐

---

## 📝 概要

> [!abstract]
> DeepSeekは2026年4月24日、フラッグシップ「V4 Pro」とその軽量版「V4 Flash」をプレビューとして公開した。V4 Proは**総パラメータ1.6兆（活性49B/トークン）**のMoEアーキテクチャを採用し、独自技術「Hybrid Attention Architecture」により最大**100万トークンコンテキスト**を実現。コーディングではLiveCodeBench **93.5%**（Claude Opus 4.6比+4.7pt）、Terminal-Bench 2.0 **67.9%**（同+2.5pt）でSOTAを塗り替えた。SWE-bench Verified **80.6%**はClaude Opus 4.6（80.8%）に0.2pt差まで迫り、出力コストは **$3.48/Mトークン**——OpenAIの$30、Anthropicの$25に対し最大9分の1という衝撃価格が業界に波紋を呼んでいる。

---

## 📊 詳細レポート

![[2026-04-24_DeepSeek-V4-Pro-Launch.svg|1600]]

---

## 🔍 特記事項

> [!note] 「1/9の価格」が意味する構造破壊
> V4 Proの単推論FLOPs消費量はDeepSeek-V3.2比**27%**、KVキャッシュも**10%**に抑制されており、低コスト化は単なるダンピングではなくアーキテクチャ上の優位によるものだ。米系ラボが$25〜$30を維持するのは、クラウドインフラ・安全審査・冗長性コストが不可避なためだが、V4 Proの普及が進めば「高い≒安全・信頼」という価値命題の再評価を迫られる。

> [!note] HybridAttention と 1Mトークン競争
> V4 ProはLinear AttentionとSelf-Attentionを交互に組み合わせた「Hybrid Attention Architecture」を採用。これにより長距離依存と局所精度を両立し、100万トークン全体を事実上1プロンプトとして扱える。コードベース全体・長大なドキュメント・会話履歴の丸ごとインジェストが可能になり、エージェント開発の設計原理が変わりうる。

> [!note] ベンチマークの「訓練データ混入」リスク
> DeepSeekのテックレポートは「GPT-5.4・Gemini 3.1-Proから3〜6か月遅れ」と自己評価するが、LiveCodeBench（93.5%）やCodeforces（レーティング3206）の突出した数値は、コーディング特化のデータキュレーションの可能性も示唆する。ベンチマーク上のSOTAと実務性能の乖離については、Hacker Newsで複数の実務エンジニアが疑義を呈している。

> [!note] Huawei Ascendチップとのエコシステム統合
> Fortuneの報道によれば、V4はHuaweiのAscend NPUとの統合を強化しており、NVIDIA H100/H200エコシステム以外でのフロンティアモデル運用という選択肢を具体化する。米国の半導体輸出規制が続く中、DeepSeekは自国インフラでも最前線モデルを動かせることを実証した形だ。

> [!note] オープンソース勢力図の塗り替え
> 1年前のV3がLlama 3.3に対抗したように、V4 ProはMeta Muse Spark（非公開）・Qwen 3.5（Alibaba）と並んで、「オープン最強」の座を三つ巴で争う構図になった。HuggingFaceでは公開直後からダウンロード数がV3.2の初週記録を超えたとの報告があり、ローカル推論コミュニティの歓迎度は高い。

---

## 🔗 関連記事

- [[2026-04-24_DeepSeek-First-Funding-20B]]
- [[2026-04-24_Tencent-Hy3-Preview]]
- [[2026-04-24_Q1-2026-VC-AI-Record]]
- [[2026-W17|📅 Week 17 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
