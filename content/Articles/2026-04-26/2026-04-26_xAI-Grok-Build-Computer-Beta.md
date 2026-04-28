---
date: 2026-04-26
category: ビジネス
source: TestingCatalog / xAI
url: https://testingcatalog.net/grok-build-and-grok-computer-xais-big-coding-push-is-finally-here/
impact: 3
tags: [AI, xAI, Grok, コーディングエージェント, エージェント, CLI]
cssclasses:
  - hide-properties
  - ai-news
---

# 🦀 xAI Grok Build & Grok Computer — ついにベータ公開

> [!tip] TL;DR
> xAIが **Grok Build**（ローカルファーストCLIコーディングエージェント）と **Grok Computer**（PCフル制御デスクトップエージェント）を同日ベータ公開。Grok Buildは **SWE-Bench Verified 70.8%**、8並列エージェント、256Kコンテキスト搭載。コードがxAIサーバーへ送信されないローカルファースト設計がプライバシー重視の企業開発者に刺さる。

> [!info] 引用元
> - 🔗 **URL**: [TestingCatalog — Grok Build and Grok Computer](https://testingcatalog.net/grok-build-and-grok-computer-xais-big-coding-push-is-finally-here/)
> - 📅 **公開日**: 2026-04-26
> - 🏷️ **カテゴリ**: #ビジネス
> - ⭐ **インパクト**: ⭐⭐⭐

---

## 📝 概要

> [!abstract]
> xAIが長らく「来週」と繰り返してきた **Grok Build** をついにライブベータで公開した。CLIバージョン 4.20.192 として公開され、モデルは `grok-code-fast-1`（256Kコンテキスト）を採用。Plan→Search→Build の3ステージワークフローで、TypeScript・Python・Java・Rust・C++・Goに対応。8つの並列エージェントを使ったArena Modeが最大の目玉で、すべてのコードはユーザーのローカル環境で実行されxAIサーバーには送信されない。同日に **Grok Computer** のベータ範囲も拡大され、PCのアプリ操作・フォーム入力・複数ステッププロセスを自律実行するデスクトップエージェントとしてSuperGrokアカウントに順次開放された。

---

## 📊 詳細レポート

![[2026-04-26_xAI-Grok-Build-Computer-Beta.svg|1600]]

---

## 🔍 特記事項

> [!note] Claude Code・Cursor との競合構図
> Grok BuildはClaude Code（Anthropic）・Cursor/Anysphere（SpaceX傘下）・GitHub Copilot（Microsoft）と直接競合する。SpaceXがAnysphereを$60B買収オプション行使で交渉中という状況下で、xAIが独自CLIを投入するのは「Musk傘下エコシステム内での競争」という異例の構図。SWE-Bench 70.8%はClaude Code（推定80%台）には届かないが、ローカル実行という差別化でニッチを狙う。

> [!note] ローカルファースト設計の意味
> コードをサーバーに送らない設計は、金融・医療・防衛等のエアギャップ環境や機密プロジェクトを持つ企業にとって決定的な差別化になりうる。一方で、クラウドベースのRAGやリアルタイム補完との組み合わせができないため、「個人開発者向け高速ツール」と「大規模コードベース解析」の間でトレードオフが生じる。

> [!note] Grok Computer の位置付けと OSWorld ギャップ
> Grok Computerは現時点でOSWorld-Verifiedのスコアが公表されておらず、Claude Mythos（79.6%）やGPT-5.5（78.7%）との比較が難しい。SuperGrok Heavy（$300/月）限定ベータであることから、一般提供前の社内品質確認フェーズとみられる。OSWorld系ベンチで競合に並ぶかどうかが公開基準になる可能性が高い。

> [!note] Grok 4.3 → Grok 5 へのつなぎ戦略
> Grok 4.3ベータ（4月17日、$300/月のSuperGrok Heavy限定）に続いてBuildとComputerを投入するのは、6Tパラメータ予定のGrok 5正式リリース前にエコシステムを整備する狙いと読める。コーディングエージェントとデスクトップエージェントで開発者ロックインを先行させ、Grok 5でフラッグシップを刷新するロードマップが透けて見える。

> [!note] 半年〜1年先の予測
> Grok Buildが70.8%という控えめなスコアでローンチしている点は、初期版としては許容範囲だが、Claude Code・Cursor・Devin（$25B評価）に対して明確なベンチマーク優位を示すことができなければエンタープライズ採用は難しい。Grok 5搭載版でSWE-Bench 85%超を達成できるかどうかが、12ヶ月以内の競争力の分水嶺になると予測する。

---

## 🔗 関連記事

- [[2026-04-25_Cognition-AI-Devin-25B-Funding]]
- [[2026-04-23_SpaceX-Cursor-60B-Option]]
- [[2026-04-26_Grok5-6T-Training-Preview]]
- [[2026-W17|📅 Week 17 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
