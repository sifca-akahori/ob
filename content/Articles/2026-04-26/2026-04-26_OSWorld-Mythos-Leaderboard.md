---
date: 2026-04-26
category: 研究
source: BenchLM.ai / Kingy AI
url: https://benchlm.ai/benchmarks/osWorldVerified
impact: 3
tags: [AI, ベンチマーク, OSWorld, Claude, Mythos, コンピュータエージェント, GPT-5.5]
cssclasses:
  - hide-properties
  - ai-news
---

# 🖥️ OSWorld-Verified 最新ランキング：Claude Mythos 79.6% で首位

> [!tip] TL;DR
> デスクトップ操作ベンチ **OSWorld-Verified** の最新ランキングで **Claude Mythos Preview が 79.6%** で首位に。Holo3-122B（78.8%）、GPT-5.5（78.7%）が僅差で追う。人間ベースライン（72.4%）を全フロンティアモデルが超え、**0.9pt 差に3モデルが密集**するという飽和に近い状況が浮き彫りに。

> [!info] 引用元
> - 🔗 **URL**: [BenchLM.ai OSWorld-Verified](https://benchlm.ai/benchmarks/osWorldVerified)
> - 📅 **公開日**: 2026-04-26
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐⭐

---

## 📝 概要

> [!abstract]
> OSWorld-Verifiedはリアルなデスクトップ環境でのタスク完了率を測定する、コンピュータエージェント評価の現在最重要ベンチマーク。最新ランキングではClaude Mythos Previewが**79.6%**でトップに立ち、ほぼ同スコアのHolo3-122B-A10B（78.8%）とGPT-5.5（78.7%）が僅差で続く。人間平均（72.4%）を7pt超えており、実務でのAIデスクトップ代替が現実味を帯びてきた。一方で、先発のGPT-5.4が3月に75.0%で人間超えを達成してから約7週間でトップ3が全モデル75%超に集中したことは、ベンチマーク自体の識別力低下を示唆する。

---

## 📊 詳細レポート

![[2026-04-26_OSWorld-Mythos-Leaderboard.svg|1600]]

---

## 🔍 特記事項

> [!note] Mythos がなぜ首位か — Project Glasswing との連動
> Claude Mythos PreviewはProject Glasswing（4/20発表）の一環として限定公開されたサイバーセキュリティ特化モデル。デスクトップ操作の精度はサイバー攻撃・防御シナリオの自動化と直結しており、OSWorldでの高スコアは「意図的な設計」の表れとも読める。Anthropicが汎用操作能力を証明したことで、Glasswingパートナー以外にも一般デスクトップエージェント市場を開拓する布石になる。

> [!note] 0.9pt 差が示す「ベンチ飽和」の問題
> 1位Mythos（79.6%）〜3位GPT-5.5（78.7%）の差はわずか0.9pt。OSWorld-Verifiedの評価スイートは実タスク369件で構成されているため、0.9ptは約3.3件の差に過ぎない。この密集は測定ノイズに近く、ベンチマーク上の「首位」が実用上の優劣と必ずしも一致しないことを示している。HN・Xでは「新しいより難しいベンチが必要」という議論が再燃している。

> [!note] Holo3-122B-A10B という謎のモデル
> 2位のHolo3-122B-A10Bは中国系AIスタートアップ Holo AIが開発した122B総パラメータ / 10B活性パラメータのMoEモデル。低い活性パラメータで高いOSWorld性能を示している点はDeepSeek V4と同様の効率化アーキテクチャを採用している可能性が高い。OSWorld以外のベンチ（MMLU・HLE等）での比較が待たれる。

> [!note] 「人間を超えた」の定義問題
> OSWorld-Verifiedの「人間ベースライン 72.4%」は**クラウドワーカーの平均パフォーマンス**に基づいており、専門的なパワーユーザーの能力ではない。「AIがデスクトップ作業で人間を超えた」という見出しは半分正確。複雑なマルチアプリ連携（例：Excelデータを元にPPTを作成しメールで送信）では、フロンティアモデルでも完了率が40〜60%程度に落ちる報告がある。

> [!note] 次の戦場は「マルチデスクトップ」か
> 現在のOSWorld-Verifiedは単一デスクトップ環境での孤立タスクが中心。半年以内に「複数のVMをまたぐマルチステップワークフロー」「Webブラウザ＋ローカルファイル統合」「エラーリカバリ率」など実業務に近い拡張版が登場すると予想される。そこでのスコアが、エンタープライズ導入判断の本当の指標になるだろう。

---

## 🔗 関連記事

- [[2026-04-20_Claude-Mythos-Project-Glasswing]]
- [[2026-04-26_GPT55-vs-Mythos-Benchmark]]
- [[2026-04-26_xAI-Grok-Build-Computer-Beta]]
- [[2026-W17|📅 Week 17 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
