---
date: 2026-05-13
category: 論文
source: SiliconANGLE / The New Stack / DataCamp
url: https://siliconangle.com/2026/05/05/subquadratic-launches-29m-bring-12m-token-context-windows-ai/
impact: 3
tags: [AI, LLM, SubQ, Subquadratic, コンテキストウィンドウ, 論文, アーキテクチャ, スパースアテンション]
cssclasses:
  - hide-properties
  - ai-news
---

# 🔢 SubQ：世界初のサブ二乗LLM——12Mトークン文脈窓・計算量1/1000・コスト1/300でClaude Opusに匹敵する精度

> [!tip] TL;DR
> Subquadratic社（元Meta生成AIヘッド Alex Whedon CTO / $29Mシード）が**世界初のフル・サブ二乗アーキテクチャLLM「SubQ」**を公開。従来のTransformerがO(n²)の計算量を要する文脈長処理を**線形O(n)に削減**するSSA（Sparse Self-Attention）を採用し、128Kトークンの長文脈ベンチ（RULER）で**Claude Opus比300倍低コスト**で同等精度（95% vs 94%）を実現。12Mトークン文脈窓は現在最大規模で、長文脈AIの経済学を根底から覆す可能性がある。

> [!info] 引用元
> - 🔗 **URL**: [Subquadratic launches with $29M to bring 12M-token context windows to AI | SiliconANGLE](https://siliconangle.com/2026/05/05/subquadratic-launches-29m-bring-12m-token-context-windows-ai/)
> - 📅 **公開日**: 2026-05-05（分析・議論は5/13にかけて継続）
> - 🏷️ **カテゴリ**: #論文
> - ⭐ **インパクト**: ⭐⭐⭐

---

## 📝 概要

> [!abstract]
> 元MetaのGenerative AIヘッドAlex Whedon（CTO）と、CEO Justin DangelがTinder共同創業者のJustin Mateen・元SoftBank Vision FundのJavier Villamizarらから2900万ドルのシードを調達して設立したSubquadratic社が、SSA（Sparse Self-Attention）ベースの独自アーキテクチャLLM「SubQ」を公開した。キービジョンは「文脈長を2倍にしてもコンピュート量が4倍になる（二乗的増加）」というTransformerの根本的ボトルネックを「2倍→2倍（線形増加）」に変えること。RULER 128Kベンチでは精度95%をわずか8ドルで達成し、同精度（94%）のClaude Opusが約2,600ドルかかる現実との対比が衝撃的だ。12Mトークン（約900万語）という文脈窓は書籍数十冊を丸ごとインプットできる規模であり、実現すれば法律・医療・研究文献の全文検索・要約ワークフローが根本的に変わる。

---

## 📊 詳細レポート

![[2026-05-13_SubQ-Subquadratic-LLM-12M-Context.svg|1600]]

---

## 🔍 特記事項

> [!note] SSA（Sparse Self-Attention）の仕組みと従来手法との違い
> 標準Transformerのアテンション機構はすべてのトークンペアを比較するため計算量がO(n²)。長文脈では文脈長が2倍になると計算量は4倍、10倍では100倍になる。SubQのSSAは「近くのトークンや選ばれた重要トークンのみを対象に注意計算を行うスパースパターン」を実装し、線形スケーリングを実現。同様のアプローチは以前もFaFa/FlashAttentionなどで試みられてきたが、SubQは「フロンティアLLMとして通用するクオリティでフル・サブ二乗を実現した初の事例」と主張している。

> [!note] コスト比較の信頼性：注意点
> 「Claude Opus比300倍安い」という主張は特定ベンチ（RULER 128K）での比較であり、タスク全般に適用できる数値ではない。また短い文脈長では標準Transformerとのコスト差はほぼ消え、SubQの利点は10万トークン超の長文脈処理に限定される。ベンチマーク自体のデザインがSubQに有利な長文脈タスクに傾いている可能性にも注意が必要。独立機関による第三者評価が待たれる。

> [!note] アーキテクチャ競争の文脈
> 2025〜2026年はMamba・RWKW・Hyena・RetNetなど「Transformerを超える」を謳うアーキテクチャが次々登場したが、いずれもフロンティアモデルとして定着するには至っていない。SubQはそれらと同じ挑戦者ポジションにある。一方、Google・Anthropic・OpenAIはFlashAttentionの改良やLinear Attentionの変種を既存モデルに取り込んでおり、SubQの差別化優位がどこまで続くかは不透明だ。

> [!note] 実用ユースケースの変化
> 12Mトークン（≈900万語）は文庫本約30〜40冊相当。M&A精査や訴訟に関わる全文書・全メール・全会議録をまとめてインプットするデューデリジェンス業務や、臨床試験全文献を一括解析するバイオ医療研究などが現実的な射程に入る。長文脈のコスト問題が消えれば、これまで「長すぎてAIに渡せなかった」文書処理ワークフローが急速に変わる。

> [!note] 半年〜1年先の予測
> SubQのアーキテクチャが成立するなら、既存大手ラボは速やかに同等アプローチをフラッグシップモデルに組み込もうとするはず（Googleはすでに研究中との報告あり）。2027年前半にはSubQ型アーキテクチャ採用モデルが複数登場し、長文脈コストが大幅低下するシナリオが有力。ただし「第三者ベンチで主張通りの性能が再現される」ことが前提条件。

---

## 🔗 関連記事

- [[2026-05-12_DeepSeek-V4-MoE-Frontier]]
- [[2026-05-13_Google-SpaceX-Orbital-Datacenter]]
- [[2026-W20|📅 Week 20 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
