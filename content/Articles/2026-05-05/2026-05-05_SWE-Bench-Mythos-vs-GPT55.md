---
date: 2026-05-05
category: 研究
source: LLM Stats / BenchLM / TokenMix
url: https://llm-stats.com/benchmarks/swe-bench-verified
impact: 2
tags: [AI, SWEbench, ベンチマーク, ClaudeMythos, GPT55, 研究, コーディングAI, リーダーボード]
cssclasses:
  - hide-properties
  - ai-news
---

# 📊 SWE-bench最前線：Mythos 93.9% vs GPT-5.5 88.7%——「使えない1位」が示すベンチ危機

> [!tip] TL;DR
> SWE-bench Verifiedリーダーボードで**Claude Mythos Preview 93.9%**がトップに立つが、一般公開されていないため実質「参照専用スコア」。開発者が実際に使える頂点は**GPT-5.5の88.7%**か**Claude Opus 4.7の87.6%**。さらにGPT-5.5はSWE-bench Pro（難易度↑）では**58.6%**に急落しOpus 4.7が逆転という「ベンチマーク分裂」が発生。「どのモデルが最強か」の答えが評価手法次第で変わるという構造問題が業界で議論を呼んでいる。

> [!info] 引用元
> - 🔗 **URL**: [LLM Stats SWE-bench Leaderboard](https://llm-stats.com/benchmarks/swe-bench-verified)
> - 📅 **公開日**: 2026-05-05
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> 2026年5月時点のSWE-bench Verifiedリーダーボードは**Claude Mythos Preview 93.9%（1位）→ GPT-5.5 88.7%（2位）→ Claude Opus 4.7 87.6%（3位）**という序列だが、Mythos Previewは一般非公開。SWE-bench Proでは順位が入れ替わり、OpusがGPT-5.5を上回る。またSWE-bench Lite（軽量版）ではClaude Opus 4.6が62.7%でトップ。同じ「コーディングAI能力」を測るはずのベンチが、変形版ごとに異なる勝者を生む現象は「ベンチマーク飽和」の予兆とも読める。2024年8月に33%だったトップスコアが2年弱で93.9%に到達した加速度は、AIコーディング能力曲線が直線ではないことを示している。

---

## 📊 詳細レポート

![[2026-05-05_SWE-Bench-Mythos-vs-GPT55.svg|1600]]

---

## 🔍 特記事項

> [!note] SWE-bench Verified vs Proの設計思想の違い
> SWE-bench Verifiedは「1,000件の人間確認済み問題」で再現性重視。SWE-bench Proは「より複雑な複数ファイル変更・長期依存性のある問題」が多く、推論とコンテキスト管理能力をより厳しく問う。GPT-5.5がVerifiedで優位でProで劣後するのは、**短い問題への最適化が長い推論チェーンに転化しない**という能力プロファイルの違い。「どの用途で使うか」によって最適モデルが異なる実用的事実。

> [!note] 「93.9%の天井」はどこにあるか
> SWE-bench Verifiedの理論上限は100%だが、実際の天井はおそらく**96〜97%**程度。残りの問題は「仕様が曖昧」「テスト自体にバグ」「人間でも複数の合法的解法が存在」するケースが含まれ、完全解決不能な問題が一定数存在する。これは「AI=人間超え」のナラティブに限界線を引く。一方、SWE-bench Proの77.8%（Mythos）には依然として大きな伸び代がある。

> [!note] ベンチマーク汚染疑惑の現実
> Hugging FaceのCTO Thomas Wolfが指摘するように、SWE-benchの問題はGitHub上の公開コードから収集されており、**訓練データとの汚染（data contamination）リスク**が指摘されている。特にGPT-5.5はOpenAI社内で広範なデータ収集が可能なため、意図せざる訓練汚染の可能性が排除できない。各社の透明性のなさが「ベンチマークへの信頼危機」を加速させている。

> [!note] 次世代評価指標への移行
> SWE-benchの飽和を受け、**SWE-bench Ultra**（推定解決時間20時間超のタスク）やTerminal-Bench（CLIフロー全体）、さらにSWE-gym（ライブリポジトリへの継続的評価）が並行して整備されつつある。AIコーディング能力の「現実の開発業務への直結度」を測るには静的ベンチマークでは限界があり、GitHubのリアルタイムIssue解決レートなど動的指標への移行が2026年後半の議題になる。

> [!note] 半年後の競争予測
> Mythos Preview相当のモデルを一般公開に近い形で展開できたラボが「コーディングエージェント市場」を制する可能性が高い。OpenAIはCodex（GPT-5.5ベース）の拡張で対抗、Google DeepMindはGemini 3.1 Pro のコーディングアリーナ首位を活かして追う。「97%の壁」を超えるモデルが2026年末か2027年Q1に登場するかどうかが注目点。

---

## 🔗 関連記事

- [[2026-05-05_Claude-Mythos-Preview-93pct-SWE]]
- [[2026-05-03_OpenAI-GPT55-Cyber-Irony]]
- [[2026-W19|📅 Week 19 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
