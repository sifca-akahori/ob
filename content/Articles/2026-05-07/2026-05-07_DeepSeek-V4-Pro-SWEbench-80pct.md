---
date: 2026-05-07
category: 研究
source: NIST CAISI / BenchLM / DataCamp
url: https://www.nist.gov/news-events/news/2026/05/caisi-evaluation-deepseek-v4-pro
impact: 3
tags: [AI, DeepSeek, V4Pro, SWEbench, MoE, ベンチマーク, オープンソース, 中国AI]
cssclasses:
  - hide-properties
  - ai-news
---

# 🚀 DeepSeek V4 Pro：SWE-bench **80.6%**・Codeforces **3,206**でOpus 4.7を**10分の1のコスト**で凌駕

> [!tip] TL;DR
> DeepSeek V4 ProがSWE-bench Verified **80.6%**・Codeforces **3,206点**を達成し、Claude Opus 4.7に肉薄しながらコストは**約1/10**。284Bパラメータ（Mixture-of-Experts）でトークンあたり**13Bのみ活性化**という設計が「知性あたりコスト」の業界最高効率を実現。NISTのCAISIが独自評価し「最も能力の高い中国産AIモデル」と認定した。

> [!info] 引用元
> - 🔗 **URL**: [NIST CAISI Evaluation](https://www.nist.gov/news-events/news/2026/05/caisi-evaluation-deepseek-v4-pro)
> - 📅 **公開日**: 2026-05-07
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐⭐

---

## 📝 概要

> [!abstract]
> DeepSeek V4 Proは284Bパラメータ・MoEアーキテクチャで、推論時に活性化するパラメータは**13B**のみ。これにより推論コストは西洋フロンティアモデルの**1/10以下**となる。SWE-bench Verified 80.6%はGPT-5.5に次ぐ公開アクセスモデル上位圏で、Codeforces 3,206はOpus 4.7を上回る。NISTのCAISIは7ベンチマークうち5つで「GPT-5.4 Miniより高コスト効率」と評価。ただし「フロンティアまで約8ヶ月の遅れ」という現実も明記されており、セキュリティコミュニティでの懸念と同時に業界の評価が分かれている。

---

## 📊 詳細レポート

![[2026-05-07_DeepSeek-V4-Pro-SWEbench-80pct.svg|1600]]

---

## 🔍 特記事項

> [!note] 284B総パラメータ・13B活性：MoEの新地平
> 「284Bだが実質13B」というMoE設計は、Dense 13Bモデルの推論コストで284Bモデルの知識量を活用できることを意味する。これはDeepSeekが2025年初頭に示したV3の設計思想を継承・発展させたもの。同等の総パラメータを全て活性化するDenseモデルと比較して**約20倍の効率差**が理論上生じる。西洋ラボがDenseモデルを主力にし続ける中、MoEの優位性がコスト競争で顕在化しつつある。

> [!note] 中国4ラボが12日間で競合モデルをリリースした意味
> GLM-5.1（Z.ai）・M2.7（MiniMax）・Kimi K2.6（Moonshot）・V4（DeepSeek）が12日間で出揃い、全てが類似のコーディング性能を示した。これは「中国AI研究コミュニティ全体が同一の技術的成熟点に到達した」ことを示唆する。競合が激化するほど公開ウェイト化が加速し、西洋フロンティアラボの「非公開優位」が侵食されるメカニズムが鮮明だ。

> [!note] CAISIの「8ヶ月遅延」評価の政治的含意
> NISTが「フロンティアから8ヶ月遅れ」と評価したことは、米国の輸出規制（EAR/エンティティリスト）がDeepSeekのチップ調達を制限しているにもかかわらず、中国が独自の最適化技術で差を縮めていることを公式に認めたに等しい。同時にCAISIが「コスト効率で米国モデルを上回る」と記したことは、輸出規制の有効性に疑問を呈す材料として使われるリスクもある。

> [!note] ベンチマークの解釈：Verified vs Pro版の乖離
> SWE-bench Verified（手動検証済みサブセット）とSWE-bench Pro（より難度の高い本番類似タスク）でスコアの序列が逆転する現象が続いている。DeepSeek V4 ProはVerified版では健闘するが、Pro版（未公開詳細）ではReasoning特化タスクでOpus 4.7に劣るとの報告がある。「どのベンチを信じるか」がますます重要な判断になってきた。

> [!note] オープンウェイトが日本・EUに与える戦略機会
> DeepSeek V4 ProはオープンウェイトであるためEU AI法のGPAI義務（8月2026年適用）の対象外となる可能性がある（発行者が中国企業のため管轄が曖昧）。日本のAI研究機関や国内ベンダーがBase ModelとしてDeepSeekを採用するケースが増加しており、次期NEDO助成においてDeepSeek系モデルをファインチューニングする計画が複数走っている。

---

## 🔗 関連記事

- [[2026-05-05_SWE-Bench-Mythos-vs-GPT55]]
- [[2026-05-05_Claude-Mythos-Preview-93pct-SWE]]
- [[2026-05-04_DeepSeek-mHC-Architecture]]
- [[2026-W19|📅 Week 19 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
