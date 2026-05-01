---
date: 2026-04-30
category: 研究
source: Alibaba Qwen / HuggingFace / r/LocalLLaMA
url: https://huggingface.co/Qwen/Qwen3.6-35B-A3B
impact: 2
tags: [AI, Qwen, Alibaba, オープンモデル, SWE-bench, コーディング, MoE, Apache2.0]
cssclasses:
  - hide-properties
  - ai-news
---

# 🐉 Qwen 3.6：SWE-Bench 73.4%でオープンウェイト・コーディング首位——r/LocalLLaMA が沸騰

> [!tip] TL;DR
> Alibaba QwenチームのQwen3.6（35B-A3B MoE）がSWE-Bench Verified **73.4%**を記録し、オープンウェイトモデルのコーディング最強に。**Apache 2.0**でリリースされ、r/LocalLLaMAで「ローカルでGPT-5.5に近い精度が出せる」と大反響。4月30日時点でHugging Faceのweeklyトレンドを独走中。

> [!info] 引用元
> - 🔗 **URL**: [HuggingFace Qwen3.6-35B-A3B](https://huggingface.co/Qwen/Qwen3.6-35B-A3B)
> - 📅 **公開日**: 2026-04-16（4月30日時点でHFトレンド首位継続）
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> Qwen3.6-35B-A3Bは35Bパラメータ・3B活性化のMoEアーキテクチャ。SWE-Bench Verified 73.4%（オープンウェイトSoTA）・SkillsBench+9.9pt・SciCode+10.8ptと複数の能力評価で大幅改善を達成。Ollama・vLLM・HuggingFaceから即日利用可能。Apache 2.0ライセンスにより商用展開・改変・ファインチューニングが完全に自由。コーディング特化の「Max-Preview」バリアントは6つの主要コーディングベンチマークで首位を主張。r/LocalLLaMAでは「家庭用GPU（RTX 4090でも量子化で動く）でGPT-5.5水準のコーディングが可能」という報告が相次ぎ、4月下旬のオープンウェイト議論のハイライトになっている。

---

## 📊 詳細レポート

![[2026-04-30_Qwen36-Open-Coding-Frontier.svg|1600]]

---

## 🔍 特記事項

> [!note] SWE-Bench 73.4%の競合文脈
> 4月30日時点のSWE-Bench Verifiedの主要スコア比較：Claude Mythos（限定公開）93.9%、DeepSeek V4 Pro 80.6%、GPT-5.5 Spud 58.6%（SWE-Bench Pro）、Qwen3.6 73.4%（オープンウェイト）。オープンウェイトで73.4%はDeepSeek V4 Flash（推定）に次ぐ水準であり、「ローカルで動くコーディングエージェント」として極めて実用的な域に達している。

> [!note] 3B活性化 MoE の経済的優位性
> 35Bパラメータ全体のうち推論時に活性化するのは約3B。これは速度・VRAM消費の観点でDense 7Bモデルに近い挙動をしながら、35Bの「知識容量」を持つことを意味する。RTX 4090（24GB VRAM）でQ4量子化（約20GB）での動作報告が出ており、月額$0のローカルコーディングエージェントが現実になった。

> [!note] 中国製オープンウェイトの「実質クローズド化」への反論
> Meta Muse SparkのクローズドSOURCE化で「中国製オープンウェイトは信頼できないのでは」という議論が持ち上がっていた中、AlbabaはQwen3.6をApache 2.0で提供。DeepSeekのオープンソース維持とともに「中国製モデルの透明性」をめぐる議論に一定の反論を提供している形。ただし学習データの透明性・政府との関係は依然として懸念事項。

> [!note] IBM Granite 4.1との比較
> 同日発表のIBM Granite 4.1とは対照的なポジショニング：Qwen3.6はSWE-Bench等の汎用コーディングで最強、Granite 4.1はエンタープライズ・表/グラフ認識・音声で特化。企業が「オープンウェイト採用」を検討する場合、用途（汎用コーディングエージェント vs 文書AI）によって選択肢が明確に分かれる状況になった。

> [!note] コミュニティ反応と半年後の予測
> r/LocalLLaMAでは「Qwen3.6がLlama 4を全カテゴリで超えた」という評価が定着しつつある。Meta Llama 4はMuse SparkのクローズドSOURCE化・ライセンス制限で人気を失い、「西側製で信頼できる代替」としてGranite 4.1、「性能最優先」としてQwen3.6という二極化が進む。半年後にはQwen4が登場すると予測されており、フロンティアとオープンウェイトの性能差がさらに縮まる可能性がある。

---

## 🔗 関連記事

- [[2026-04-27_OpenSource-AI-Frontier-Gap-Closing]]
- [[2026-04-24_DeepSeek-V4-Pro-Launch]]
- [[2026-04-30_IBM-Granite-4-1-Release]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
