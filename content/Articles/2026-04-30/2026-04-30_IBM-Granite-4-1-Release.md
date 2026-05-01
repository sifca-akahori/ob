---
date: 2026-04-30
category: 研究
source: IBM Research Blog / Hugging Face / GIGAZINE
url: https://research.ibm.com/blog/granite-4-1-ai-foundation-models
impact: 2
tags: [AI, IBM, Granite, オープンモデル, 企業AI, Apache2.0, 効率化]
cssclasses:
  - hide-properties
  - ai-news
---

# 🪨 IBM Granite 4.1リリース：8BモデルがMoE 32Bに匹敵——Apache 2.0で3サイズ全公開

> [!tip] TL;DR
> IBMが**Granite 4.1**を4月30日に公開。**3B・8B・30B**の3サイズ（Dense・Instruct）＋Speech 4.1（ASR+翻訳）＋Vision 4.1（表・グラフ認識）を**Apache 2.0**でリリース。8Bモデルが**旧世代MoE 32Bに匹敵**する性能を達成し、HNで「エンタープライズOSSの新スタンダードになれる」と195pt・105コメントを集めた。

> [!info] 引用元
> - 🔗 **URL**: [IBM Research Blog](https://research.ibm.com/blog/granite-4-1-ai-foundation-models)
> - 📅 **公開日**: 2026-04-30
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> IBMは4月30日、Granite 4.1シリーズを発表。目玉は**8Bモデルが旧Granite 4.0の32B MoEモデルに匹敵**するという劇的な効率改善で、約**15兆トークン**のマルチフェーズ学習で達成。全モデルはApache 2.0（商用・改変自由）。さらにGranite Speech 4.1（多言語ASR・翻訳、エッジ向け2Bモデル×2）とGranite Vision 4.1（4Bパラメータで表・グラフ認識においてClaude Opus 4.6を超えると主張）を同時公開。Hacker Newsでは195pt・105コメントと高い注目を集めた。

---

## 📊 詳細レポート

![[2026-04-30_IBM-Granite-4-1-Release.svg|1600]]

---

## 🔍 特記事項

> [!note] 「8B が MoE 32B に匹敵」の技術的意味
> MoE（Mixture of Experts）はパラメータ総数は多いが活性パラメータは少ないアーキテクチャで、Mixtral・DeepSeek等が採用。Dense 8Bがそれに匹敵するとは、計算効率・パラメータ活用率で大幅な改善があったことを示す。背景には15兆トークンの段階的学習（広範なプリトレーニング→高品質技術・数学データへのアニーリング）があり、データキュレーションとトレーニング手法の成熟を示す。

> [!note] Apache 2.0の戦略的意義
> Llama 4（Metaカスタムライセンス）やGemma 3（制限付き）と異なり、Apache 2.0は商用利用・改変・再配布が完全に自由。企業のオンプレミス展開・ファインチューニング・API商用化に障壁がない。IBMは「AI信頼性・コスト・コンプライアンスの3点でエンタープライズ最適」というポジショニングを強化しており、オープンウェイト競争でLlama 4の弱点（ライセンス制限）を直接突く。

> [!note] Vision 4.1「Claude Opus 4.6を超える」主張の評価
> IBMが「表・グラフ認識でClaude Opus 4.6を超える」と主張するが、これは特定ベンチマーク（表・グラフ特化）での比較であり、汎用視覚理解の比較ではない。ただしドキュメントAI（財務諸表・報告書解析）という実務タスクで最先端に匹敵するなら、エンタープライズ導入の意思決定に直接影響する。4Bという小型モデルで実現している点も評価に値する。

> [!note] Speech 4.1のエッジAI戦略
> 2Bモデル×2（自己回帰ASR+非自己回帰編集）というデュアル設計は、精度の高い書き起こし（自己回帰）と高速推論（非自己回帰）を切り替えられる実用的設計。エッジデバイス（病院・工場・モバイル端末）での多言語音声AI展開を想定しており、Whisper系の代替として企業採用が見込める。

> [!note] オープンウェイト競争の文脈
> Qwen 3.5（中国）・DeepSeek V4 Flash・GLM5とともに、Granite 4.1は「西側企業製オープンウェイトのエンタープライズ向け選択肢」として位置づく。4月下旬の流れを見ると、オープンウェイトがフロンティアモデルとの性能差を急速に縮める段階に入っており、「API課金モデル」と「自社ホスティング」の経済比較が企業の意思決定の核心になりつつある。

---

## 🔗 関連記事

- [[2026-04-27_OpenSource-AI-Frontier-Gap-Closing]]
- [[2026-04-24_DeepSeek-V4-Pro-Launch]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
