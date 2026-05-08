---
date: 2026-05-08
category: ビジネス
source: Google DeepMind / Google Cloud Blog
url: https://cloud.google.com/blog/products/ai-machine-learning/gemini-3-1-flash-lite-is-now-generally-available
impact: 2
tags: [AI, Google, Gemini, モデルリリース, コスト効率, API, Flash]
cssclasses:
  - hide-properties
  - ai-news
---

# ⚡ Gemini 3.1 Flash-Lite GA：$0.25/1Mトークン・356トークン/秒・GPQA 86.9%——コスパ最強の量産モデル

> [!tip] TL;DR
> GoogleのGemini 3.1 Flash-Liteが**正式GA（2026-05-07）**。入力**$0.25/1Mトークン**・出力$1.50/1Mトークンという最低水準の価格で、**356トークン/秒**（Gemini 2.5 Flash比2.5倍速）・**GPQA Diamond 86.9%**・Arena Elo **1432**を達成。「Gemini 2.5 Flash相当の品質を1/4のコスト以下で」という明快なポジショニングで、API規模展開・RAGパイプライン・モバイルエッジ等の大量処理用途を狙う。

> [!info] 引用元
> - 🔗 **URL**: [Google Cloud Blog](https://cloud.google.com/blog/products/ai-machine-learning/gemini-3-1-flash-lite-is-now-generally-available)
> - 📅 **公開日**: 2026-05-07
> - 🏷️ **カテゴリ**: #ビジネス
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> Googleは5月7日、Gemini 3.1 Flash-Liteの一般提供（GA）を開始した。2026年3月にプレビュー提供が始まったフラッシュ系最軽量モデルで、前世代（Gemini 2.0 Flash-Lite）比でGPQA Diamond 86.9%・MMMU Pro 76.8%という大幅な精度向上を実現しながら、価格は$0.25（入力）/$1.50（出力）と1Mトークン単位で業界最安水準を維持。Artificial Analysis社のベンチマークでは356トークン/秒・Time to First Token（TTFT）2.5倍改善を記録。品質指標はGemini 2.5 Flash（非Lite）と同等とされており、「高品質×高速×低コスト」という三角形を実現したと主張する。

---

## 📊 詳細レポート

![[2026-05-08_Gemini-31-Flash-Lite-GA.svg|1600]]

---

## 🔍 特記事項

> [!note] 「Gemini 2.5 Flash相当の品質」という主張の検証
> GoogleはFlash-LiteがGemini 2.5 Flash相当とするが、Artificial Analysis等の独立評価ではIntelligence Index 34（対象モデル中央値：21）という水準に留まっており、GPQA Diamond 86.9%はフラッグシップ（Mythos 94.6%・Gemini 3.1 Pro推定）に比べれば大幅に劣る。「Lite」ラインが狙う用途（大量RAG・分類・要約）ではこの精度で十分なケースが大半だが、「Gemini 2.5 Flash相当」の主張は異なる条件下で実施されたベンチマークの選択的引用の可能性を念頭に置く必要がある。

> [!note] GPT-5.5 Instantとの競合構図
> 同週にChatGPTデフォルトになったGPT-5.5 Instantは高品質エンドポイントとして位置付けられているのに対し、Flash-Liteはその下位の「大量処理」カテゴリを狙う。直接の競合はMeta Llama 4 Scout（OSS）・Mistral Small 3.1（OSS）・Claude Haiku 4.5（Anthropic）。価格帯ではFlash-Liteが最も攻撃的な設定をしており、特にGoogle Cloudを既に使用しているエンタープライズ顧客に対してはVertex AIとのネイティブ統合という強力な粘着要因がある。

> [!note] モバイル・エッジへの展開戦略
> Flash-Liteの356トークン/秒という高速出力はサーバーサイド推論の数字だが、GoogleはGemini Nanoとの組み合わせでオンデバイス（Pixel・Android）での活用も視野に入れている。特にAndroid 16での「AIアクセシビリティレイヤー」統合にFlash-Liteのクラウドエンドポイントが使われるシナリオが噂されており、Pixel 10発売（2026年秋予定）前の地盤固めとも解釈できる。

> [!note] コスト破壊とAIの民主化
> $0.25/1M入力トークンは2024年のGPT-3.5-turboとほぼ同価格で、GPQA Diamond 86.9%という精度を提供する。2023年時点で86.9%のGPQA Diamond達成には$100/1Mトークン級のコストが必要だった。この3年間での精度/コスト比改善は100倍以上に達しており、「フロンティア品質へのアクセス民主化」が急速に進んでいることを示す。同時に、この価格下落はAIラボの収益性圧迫（モデル提供はコストセンター化）という逆説を進行させている。

> [!note] 1年後の予測
> Flash-Liteは2027年以降、さらにFlash-Nanoまたは量子化版として端末組み込みを狙う方向で進化する可能性が高い。一方でAPI価格は業界全体でさらに50〜70%下落する見込みであり、「$0.25/1Mトークン」も2027年末には競合の新参入によって陳腐化するだろう。Google DeepMindの真の優位は価格ではなく、Gemini Ultra・Pro・Flash・Liteというラインナップ全体と、Google検索・Workspace・Android・CloudとのエコシステムのTight統合にある。

---

## 🔗 関連記事

- [[2026-05-07_GPT55-Instant-OSWorld-75pct]]
- [[2026-05-06_OpenAI-GPT55-Instant-Default]]
- [[2026-05-08_OpenAI-Agent-Phone-2027-MediaTek-2nm]]
- [[2026-W19|📅 Week 19 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
