---
date: 2026-05-03
category: 研究
source: NIST CAISI
url: https://www.nist.gov/news-events/news/2026/05/caisi-evaluation-deepseek-v4-pro
impact: 2
tags: [AI, DeepSeek, NIST, CAISI, 評価, ベンチマーク, 中国AI, 安全保障]
cssclasses:
  - hide-properties
  - ai-news
---

# 🔭 DeepSeek V4 Pro CAISI/NIST独立評価：「フロンティアから8ヶ月遅れ」——数学は例外的に同等

> [!tip] TL;DR
> 米国NIST傘下のAI安全研究所（CAISI）がDeepSeek V4 Proを独立評価。全体的なフロンティアモデル比較で**「8ヶ月遅れ」**と結論付けたが、**数学ベンチではGPT-5.5と統計的同等**という注目すべき例外を発見。LiveCodeBench 93.5・Codeforces ELO 3,206（GPT-5.5の3,168を上回る）のコーディング性能も際立つ。DeepSeekの自己申告「フロンティア同等」に公的機関が初めて疑問符を付けた。

> [!info] 引用元
> - 🔗 **URL**: [NIST CAISI Evaluation](https://www.nist.gov/news-events/news/2026/05/caisi-evaluation-deepseek-v4-pro)
> - 📅 **公開日**: 2026-05（週末に注目集まる）
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> NSTのComprehensive AI Safety Institute（CAISI）がDeepSeek V4 Proを包括的に評価し、報告書を公表した。同モデルは2026年4月24日にDeepSeekが1.6兆パラメータ（49B常時活性化）のMoEとして公開し、「米国フロンティアモデルと同等」と自己申告していた。CAISIの独立評価では7つの主要ベンチマークのうち5つでコスト効率優位を認めたが、AGIグレードの推論タスク全体では約8ヶ月の能力ギャップが存在すると結論付けた。数学（AIMEやGPQA数学分野）だけはGPT-5.5・Claude Opus 4.7と統計的差なし。MoEによる推論コスト大幅削減はDeepSeek V4 Flash（$0.07/$0.28/1Mトークン）で示されており、コスト効率面の優位性は本物だと評価された。

---

## 📊 詳細レポート

![[2026-05-03_DeepSeek-V4-NIST-Evaluation.svg|1600]]

---

## 🔍 特記事項

> [!note] 「8ヶ月遅れ」の定義と測定限界
> CAISIの「8ヶ月遅れ」は能力推定曲線上の位置で定義されており、具体的には「2025年9月時点の米国フロンティアモデルと同水準」という意味。ただし能力曲線の傾きや定義は非公開部分が多く、評価タスクの選定バイアス（英語中心・米国文化依存）が中国モデルを過小評価する可能性は複数の研究者が指摘している。

> [!note] 数学とコーディングの「強さ」の政策的含意
> 数学・コーディング能力が同等というのは安全保障上の重要サインで、これらのスキルが暗号解析・セキュリティ脆弱性発見・兵器設計等に直結するため。中国モデルが意図的にこれらの分野に特化してリソースを集中させているとしたら、「全体的遅れ」と「特定能力の同等」の組み合わせは評価手法の再設計を迫るものになる。

> [!note] DeepSeek自己申告との乖離——マーケティングとしてのベンチマーク
> DeepSeekはSWE-bench Verified 80.6%（Claude Opus 4.7の80.8%と統計的同等と主張）を大きく宣伝したが、CAISIはこれを「特定ベンチへの過適合」と示唆した。LLM評価のゲーム化は業界全体の問題で、独立機関による評価が決定的に重要になっているが、CAISI自体も「米国政府機関」という利益相反の疑いを持たれる立場にある。

> [!note] V4 Flashのコスト競争力は本物
> V4 Pro（$2.19/$8.76/1Mトークン）よりむしろV4 Flash（$0.07/$0.28）が市場インパクトは大きい。GPT-5.4 mini比でほとんどのベンチで同等かつ53%安い、という評価はCAISIも認めており、中間品質のAPIコスト競争を根本から変えている。日本企業にとっては「特化用途のClaude Haikuより安くできる選択肢」として現実的。

> [!note] 次の焦点——V4 Ultra（未公開）の存在
> DeepSeekは公式には認めていないが、HuggingFace上に「V4 Ultra」のプレースホルダが確認されており、r/LocalLLaMAでは「フロンティア完全追いつきモデル」の存在が噂されている。CAISIが「8ヶ月遅れ」と測定したタイミングでより強力なモデルが登場すれば、政策評価の前提が崩れる。

---

## 🔗 関連記事

- [[2026-04-27_OpenSource-AI-Frontier-Gap-Closing]]
- [[2026-05-03_Pentagon-Anthropic-Exclusion]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
