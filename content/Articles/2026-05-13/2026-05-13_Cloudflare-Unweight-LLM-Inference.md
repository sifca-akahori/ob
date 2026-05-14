---
date: 2026-05-13
category: 研究
source: Cloudflare Blog / InfoQ
url: https://blog.cloudflare.com/high-performance-llms/
impact: 2
tags: [AI, Cloudflare, LLM推論, インフラ, Unweight, KVキャッシュ, 最適化]
cssclasses:
  - hide-properties
  - ai-news
---

# ⚡ Cloudflare「Unweight」：無損失22%LLMフットプリント削減＋プリフィル・デコード分離で推論スループット最大化

> [!tip] TL;DR
> CloudflareがエッジネットワークでのLLM推論を大幅に効率化する2つの技術を公開した。**「Unweight」**（独自開発のロスレス推論時圧縮で**モデルフットプリントを22%削減**）と、プリフィル段階とデコード段階を別サーバーに分離する**「Disaggregated Prefill/Decode」**（KVキャッシュヒット率60%→80%）だ。GPUメモリ帯域の逼迫が最大ボトルネックとなる現在のLLMデプロイメント現場に刺さる実装技術の公開。

> [!info] 引用元
> - 🔗 **URL**: [Building the foundation for running extra-large language models | Cloudflare Blog](https://blog.cloudflare.com/high-performance-llms/)
> - 📅 **公開日**: 2026-05-13
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> Cloudflareは自社のグローバルエッジネットワーク上でLLMを効率的に動かすために開発した推論最適化技術をブログで詳述した。最大のハイライトは「Unweight」——モデルの精度を落とさずに推論時のGPUメモリ使用量を22%削減するロスレス圧縮システムだ。これによりCloudflareのグローバルGPUネットワークでより低コスト・高速なLLM推論が可能になる。加えて、入力テキストの処理（プリフィル）と応答生成（デコード）を分離した専用サーバーで処理する「Disaggregated Prefill/Decode」を実装し、KVキャッシュのヒット率をピーク時に60%から80%に改善した。Cloudflareの手法は、数百億ドルを投じてGPUクラスターを構築するのとは対照的に、エッジネットワークの分散特性を最大限に活かす「効率化戦略」だ。

---

## 📊 詳細レポート

![[2026-05-13_Cloudflare-Unweight-LLM-Inference.svg|1600]]

---

## 🔍 特記事項

> [!note] Unweightの仕組みと競合との差異
> 一般的なモデル量子化（int8・fp4化）は精度を犠牲にするため、高精度が求められるフロンティアモデルには使いにくい。Unweightは「推論時のみモデル重みを一時的に圧縮し、演算前に解凍する」という手法により、精度を保ったままGPUのHBM（High-Bandwidth Memory）フットプリントを削減する。HBMへのデータ転送がLLM推論のボトルネックである現在、この22%削減はスループット向上に直結する。

> [!note] Disaggregated Prefill/Decodeのインパクト
> プリフィル（入力処理）は計算集約的（Compute-bound）、デコード（出力生成）はメモリ帯域集約的（Memory-bandwidth-bound）という正反対の特性があるため、同一GPU上での処理は非効率だ。分離することで各段階に特化したGPU設定が可能になる。KVキャッシュヒット率の60%→80%改善は、同一プロンプトプレフィックスを持つリクエスト（APIラッパー・チャットボットなど）でコンピュート節約効果が大きい。

> [!note] Cloudflareの「第三のアプローチ」
> AIインフラは現在「GPU密集型クラスター（NVIDIA×大手クラウド）」vs「カスタムチップ（Google TPU・Anthropic Custom Silicon）」の二択が主流だが、CloudflareはStarlink的な分散エッジ戦略を採る。世界310都市超にPoP（Points of Presence）を持つCloudflareにとって、推論を最寄りのエッジで処理する低遅延モデルはアーキテクチャ的な強みになりえる。

> [!note] 競合他社との比較
> Akamaiも同週にLLM推論向けインフラの大型契約を締結（Akamai surges on big LLM deal）しており、Cloudflare株は一時下落した。CDN・エッジコンピューティング事業者がLLM推論の「ラストマイル」を争う構図が鮮明になっている。Unweightのオープンソース化や他ベンダーへのライセンス供与があればゲームチェンジャーになりうる。

> [!note] 半年〜1年先の予測
> Cloudflareは「Workers AI」プラットフォームを介してエッジLLM推論をAPIとして提供中。Unweightと分離プリフィルの組み合わせが安定稼働を実証できれば、2026年Q4〜2027年Q1に他の大手エッジプロバイダーが類似技術を追随するか、CloudflareのAPI利用者が急増するかのどちらかが起きる。SubQの12Mトークン文脈窓との組み合わせが実現すれば、エッジでの超長文脈推論という新ユースケースが開花する。

---

## 🔗 関連記事

- [[2026-05-13_SubQ-Subquadratic-LLM-12M-Context]]
- [[2026-05-12_AMD-CPU-Renaissance-Agentic-AI]]
- [[2026-W20|📅 Week 20 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
