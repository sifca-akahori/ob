---
date: 2026-04-27
category: 研究
source: Latent Space / r/LocalLLaMA / Hugging Face Blog
url: https://www.latent.space/p/ainews-top-local-models-list-april
impact: 2
tags: [AI, オープンソース, Qwen3, GLM5, DeepSeek, Meta, Llama, ローカルLLM, オープンウェイト]
cssclasses:
  - hide-properties
  - ai-news
---

# 🌐 オープンウェイトAI の逆襲：Qwen3・GLM5 が Llama 4 を超える

> [!tip] TL;DR
> 2026年4月、**オープンウェイトモデルとプロプライエタリモデルの差が急速に縮まっている**。r/LocalLLaMAコミュニティでの総意：**Qwen 3.5** がほぼ全用途で最推奨、**GLM-5**（Zhipu AI）と**DeepSeek V4 Flash**がLlama 4を汎用知識・コーディングで上回る。HuggingFaceの「Spring 2026 State of Open Source AI」レポートは**オープンソースモデル数が6ヶ月で3.7倍**に急増したことを報告。Meta の Muse Spark クローズドソース化がコミュニティに衝撃。

> [!info] 引用元
> - 🔗 **URL**: [AINews Top Local Models List April 2026 — Latent Space](https://www.latent.space/p/ainews-top-local-models-list-april)
> - 📅 **公開日**: 2026-04-27
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> Latent SpaceのSwyxとAlessioが4月版「Top Local Models」リストを公開。r/LocalLLaMA コミュニティのアップボートデータと実際のベンチマークを組み合わせた総合評価で、**Qwen 3.5**（Alibaba、70B・32Bバリアント）が汎用・コーディング・多言語の全カテゴリでトップに。**Zhipu AI の GLM-5**（120B）はGPQA・MMLUで Llama 4 Scout を平均8pt上回る。**DeepSeek V4 Flash**は出力コスト $0.38/Mトークンで量・質ともにコスパ最強と評価。一方でMetaがMuse Sparkをクローズドソースで公開したことへの反発が広がっており、コミュニティの「Llamaへの信頼が揺らいでいる」という声が増加。HuggingFaceのSpring 2026レポートでは6ヶ月でオープンモデル数が3.7倍（18K → 67K）に膨らんでいることが判明。

---

## 📊 詳細レポート

![[2026-04-27_OpenSource-AI-Frontier-Gap-Closing.svg|1600]]

---

## 🔍 特記事項

> [!note] Qwen 3.5 がなぜこれほど強いか
> Alibabaは潤沢な中国国内トレーニングデータ（中国語・数学・コーディング）に加え、DPO・PPO・GRPO等の強化学習手法を積極的に採用。特に数学・コーディングにおける精度向上は「データ量ではなくRL品質」が差をつけているとされる。Qwen 3.5の訓練コストはGPT-5クラスの1/15以下と推定され、コストあたり性能で他を圧倒。

> [!note] MetaのMuse Spark クローズドソース化の衝撃
> Metaはこれまで「オープンソースの守護者」としてLlamaシリーズを無償公開し、r/LocalLLaMAの事実上の主役だった。Muse Sparkがクローズドになったことで「MetaはLlamaを諦めた」「競争に負けて方針転換した」という不満がコミュニティに充満。ただし「Llama 5は2026後半に予定されており完全撤退ではない」とする楽観的見方もある。

> [!note] オープンウェイトの「3.7倍」の中身
> HuggingFaceの67K公開モデルのうち、実際に実用水準（汎用QA正解率60%以上）を満たすものは約12%という分析もある。多くは既存モデルのfinetuneやLoRAアダプタで、真の「新アーキテクチャ」はごく少数。数字の膨張がコミュニティの「本当に使えるモデル」探しを難しくしているという問題も浮上している。

> [!note] ローカルLLM推論インフラの成熟
> Ollama・LM Studio・Jan・GPT4AllなどのローカルLLM実行ツールの完成度が急上昇している。Apple Silicon（M3 Ultra・M4 Max）でのQwen 3.5-32B動作が実用水準に達し、「クラウドAPIなしでフロンティアに近い性能」が個人レベルで実現。これがオープンウェイトモデルの需要をさらに押し上げる正のフィードバックループを形成。

> [!note] 半年後の予測：オープン vs クローズドの新均衡
> 2026後半、Llama 5（Meta）・Falcon 3（TII）・Gemma 4（Google）がリリースされれば再びオープン陣営が勢力を盛り返すと予測される。ただし中国系モデル（Qwen・DeepSeek・GLM）が西側のオープン主要勢を性能・コストで上回る状況が続けば、輸出規制・安全保障上の懸念から使用禁止令が出るリスクも国際的に高まる。

---

## 🔗 関連記事

- [[2026-04-24_DeepSeek-V4-Pro-Launch]]
- [[2026-04-26_MemPalace-47K-Stars-Benchmark]]
- [[2026-04-26_OpenClaw-347K-GitHub-Record]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
