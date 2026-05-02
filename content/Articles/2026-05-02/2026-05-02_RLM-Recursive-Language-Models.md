---
date: 2026-05-02
category: 研究
source: Prime Intellect / arXiv
url: https://www.primeintellect.ai/blog/rlm
impact: 2
tags: [AI, RLM, LLM, コンテキスト管理, エージェント, 長期タスク, パラダイム転換]
cssclasses:
  - hide-properties
  - ai-news
---

# 🔄 Recursive Language Models（RLM）：コンテキストウィンドウを破壊する「再帰LLM」——2026年のパラダイム候補

> [!tip] TL;DR
> Prime Intellectが提唱する **Recursive Language Models（RLM）** が注目を集めている。従来のLLMがコンテキストウィンドウに縛られるのに対し、RLMはモデル自身が**Python REPLを操作して自分のコンテキストを能動的に管理**し、再帰的な自己呼び出しと外部ツールへの委譲で**理論上無制限の長期タスク**を処理する。「Bitter Lesson（大規模計算が勝つ）」に則り**訓練段階から組み込む**設計が差別化点。週単位・月単位タスクを自律処理するエージェントの実現に向けた有力アーキテクチャ候補。

> [!info] 引用元
> - 🔗 **URL**: [Prime Intellect – Recursive Language Models: the paradigm of 2026](https://www.primeintellect.ai/blog/rlm)
> - 📅 **公開日**: 2026-05-02
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> NYU PhD学生のAlex ZhangがMIT Blueprint論文（2025年10月）として提唱し、Prime IntellectがRLMEnvとして実装・普及させている**Recursive Language Models（RLM）**が2026年前半に改めて注目されている。従来のLLMはプロンプトを直接ニューラルネットに入力するが、RLMはプロンプトを**Pythonサンドボックスの変数**として外部に置き、モデルがコードを書いて「一部を参照→分解→再帰的に自己呼び出し→サブLLMに委譲」という処理をする。コンテキスト要約（情報損失が生じる）を一切行わず、**能動的なコンテキスト管理**を実現する。Prime Intellectはこれを「強化学習でRLMスカフォールディングごと訓練できる」環境として整備。数週間〜数ヶ月に及ぶ長期エージェントタスクを可能にする実装基盤として、オープンソースの「rig RLM library」がGitHubで公開されている。

---

## 📊 詳細レポート

![[2026-05-02_RLM-Recursive-Language-Models.svg|1600]]

---

## 🔍 特記事項

> [!note] 「要約しない」という哲学——情報損失ゼロの長期記憶へ
> 既存の長コンテキスト解決策（RAG・スライディングウィンドウ・圧縮要約）は本質的に情報損失を伴う。RLMが「コンテキストを外部オブジェクトとして扱い、モデルがコードで操作する」設計は、人間の脳が「ノートにメモして必要なときに参照する」認知方式に近い。LOCOMO ベンチマーク（4/27記事）で全主要LLMがナイーブRAGに敗北したことを踏まえると、**RLMのアプローチは現行のRAG限界を突破する**可能性がある。

> [!note] 「Bitter Lesson」への準拠——スカフォールディングを訓練に組み込む
> Rich Suttonの「Bitter Lesson（スケールと計算が手作りのヒューリスティックに勝つ）」に従い、RLMはRLMスカフォールディング（Python REPL管理ループ）を推論時の後付けではなく**訓練段階から組み込む**。これにより「コンテキスト折りたたみ（learned context folding）」が訓練で洗練されていく。現在主流のReAct/Functionコール型エージェントが「訓練後にツール使用を貼り付ける」構造と本質的に異なる。

> [!note] 競合アーキテクチャとの比較——Mamba・RWKV・TTTとの棲み分け
> 長期コンテキスト問題を解く別アプローチとして、State Space Models（Mamba 2）・Linear Attention（RWKV）・Test-Time Training（TTT）がある。これらは**アーキテクチャレベル**での解決を目指すが、RLMはTransformerを変えずに**推論・訓練パラダイムレベル**での解決を試みる。相互補完の余地があり「Mamba+RLM」のような組み合わせも理論上可能。ただし現在RLMの実測ベンチマーク（特に長期実タスク）はまだ限られており、夢物語終わりを防ぐためにも実証が必要。

> [!note] エンタープライズAIエージェントとの接続——OutSystems報告との共鳴
> 4/29の記事（エンタープライズAIエージェント普及率96%・管理プラットフォーム保有12%）と重ねると、RLMが解こうとしている課題は「長期エージェントがいかに状態を管理するか」という現場の痛点に直結している。CRMや業務システムをまたがる週単位のエージェントワークフローには、現在のセッションベースLLMでは対処しきれない。RLMが成熟すれば、まずエンタープライズ向け「永続エージェント」として市場に出てくる可能性が高い。

---

## 🔗 関連記事

- [[2026-04-27_LOCOMO-Agent-Memory-Benchmark]]
- [[2026-04-29_Enterprise-AI-Agent-Sprawl]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
