---
date: 2026-04-26
category: 研究
source: Kingy AI / BenchLM.ai
url: https://kingy.ai/ai/claude-mythos-preview-vs-gpt-5-5-a-benchmark-by-benchmark-showdown-between-the-two-most-important-frontier-models-of-april-2026/
impact: 2
tags: [AI, ベンチマーク, Claude, Mythos, GPT-5.5, OpenAI, Anthropic, 比較]
cssclasses:
  - hide-properties
  - ai-news
---

# 📊 GPT-5.5 vs Claude Mythos：4月の頂上決戦ベンチ比較

> [!tip] TL;DR
> 4月最重要の2モデル **GPT-5.5**（API公開済み）と **Claude Mythos Preview**（限定公開）の主要ベンチ比較が出揃った。数学・コーディングでは GPT-5.5 がリード（FrontierMath **39.6%** vs Mythos未公表、SWE-Bench Pro **58.6%**）、デスクトップ操作では Mythos が首位（OSWorld **79.6%** vs GPT-5.5 **78.7%**）。総合的には「どちらが上か」は測定軸に依存し、**コスト面では GPT-5.5 が 2倍の価格差**という選択の分岐点がある。

> [!info] 引用元
> - 🔗 **URL**: [Kingy AI — Claude Mythos vs GPT-5.5](https://kingy.ai/ai/claude-mythos-preview-vs-gpt-5-5-a-benchmark-by-benchmark-showdown-between-the-two-most-important-frontier-models-of-april-2026/)
> - 📅 **公開日**: 2026-04-26
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> 4月に登場した最重要2フロンティアモデル、OpenAI の **GPT-5.5**（4/23リリース・API開放済み）と Anthropic の **Claude Mythos Preview**（4/20発表・限定公開）の包括的ベンチマーク比較が公開された。GPT-5.5 は数学（FrontierMath 39.6%）・コーディング（SWE-Bench Pro 58.6%、Terminal-Bench 2.0 82.7%）で優位を示す一方、OSWorld-Verified（デスクトップ操作）では Mythos 79.6% が GPT-5.5 78.7% をわずかに上回る。HLE（Humanity's Last Exam）では Mythos が 41.2% と GPT-5.5 の 40.8% を僅差でリード。API 価格は GPT-5.5 が $5/$30（入出力/1Mトークン）で、Claude Opus 4.7 の約2倍。コスト効率を重視するなら Claude Opus 4.7、最高性能を追うなら GPT-5.5 という選択構図が浮き彫りになった。

---

## 📊 詳細レポート

![[2026-04-26_GPT55-vs-Mythos-Benchmark.svg|1600]]

---

## 🔍 特記事項

> [!note] Mythos が「限定公開」である不公平さ
> 比較の前提として、Claude Mythos Preview は Project Glasswing 経由の限定パートナーのみがアクセス可能であり、一般の開発者は評価できない。公開されているベンチスコアは Anthropic 側の自己報告ベースが多く、独立した再現実験が困難。GPT-5.5 は API で誰でも評価できるため、コミュニティの検証数で圧倒的優位にある。「公平な比較」という観点では、Mythos の数字には割引が必要だという意見がある。

> [!note] FrontierMath の意義と限界
> GPT-5.5 の FrontierMath 39.6% は Claude Opus 4.7（23.2%）の約1.7倍という圧倒的差。FrontierMath は数学オリンピック・数論・解析学など専門家レベルの問題を収録しており、LLMの「真の数学的推論」を測定する試みとして高く評価されている。ただし問題セットに生成AI訓練データが含まれているかどうかの検証が不十分という批判もある。

> [!note] 「コーディングで GPT-5.5 が勝つ」の実態
> SWE-Bench Pro 58.6% はコーディングエージェントとして高いが、DeepSeek V4-Pro の 55.4%（$3.48/1M出力）と比較すると**価格対性能は大きく劣る**。API価格 $30/1M出力の GPT-5.5 はDeepSeekの9倍の価格を払っても精度差は約3pt。コスト感応度が高いスタートアップや研究機関にとって、「最高性能」の選択は合理的でない場面が多い。

> [!note] 「総合的にどちらが優れているか」への答え
> 結論は「ユースケース次第」で、コーディング・数学・アシスタント：GPT-5.5、デスクトップエージェント・サイバーセキュリティ：Mythos、コスト効率：Claude Opus 4.7 または DeepSeek V4、オープンソース利用：DeepSeek V4 Flash という整理になる。単一モデルで「全てで最強」は存在せず、ユースケース特化の選択が2026年のデプロイ実務の実態。

> [!note] 半年後のモデル地図予測
> GPT-5.5 と Mythos Preview の対決は「暫定王者争い」に過ぎない。Grok 5（6T params, Q2-Q3）、Claude 5（H2予定）、Gemini 3.2（開発中）が登場することで現在のランキングは刷新される。注目すべきは「推論時計算（TTC）の効率化」と「マルチモーダル・エージェント統合」の2軸であり、そこで差をつけたモデルが次の12ヶ月の市場をリードすると予測する。

---

## 🔗 関連記事

- [[2026-04-26_OSWorld-Mythos-Leaderboard]]
- [[2026-04-23_GPT-5-5-Spud-Release]]
- [[2026-04-24_DeepSeek-V4-Pro-Launch]]
- [[2026-W17|📅 Week 17 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
