---
date: 2026-05-03
category: 研究
source: Mistral AI
url: https://mistral.ai/news/vibe-remote-agents-mistral-medium-3-5
impact: 3
tags: [AI, Mistral, LLM, オープンウェイト, SWE-bench, コーディング, Medium35, Vibe]
cssclasses:
  - hide-properties
  - ai-news
---

# 🌊 Mistral Medium 3.5：128B Dense統合フラッグシップ、SWE-bench 77.6%でオープン最高水準

> [!tip] TL;DR
> MistralがMedium 3.1とMagistral推論モデルを**一本化**した128B Denseフラッグシップ「Medium 3.5」を公開。**SWE-bench Verified 77.6%**（オープンモデル最高水準）を記録し、Vibe CLIには非同期クラウドエージェントを統合。改訂MIT準拠ライセンスで4GPU自己ホスト可能、API $1.50/$7.50（入出力/1Mトークン）の価格にはHNで批判も。

> [!info] 引用元
> - 🔗 **URL**: [Mistral AI](https://mistral.ai/news/vibe-remote-agents-mistral-medium-3-5)
> - 📅 **公開日**: 2026-04-29（週末に拡散）
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐⭐

---

## 📝 概要

> [!abstract]
> Mistral AIが128Bパラメータ・256Kコンテキストウィンドウの「Medium 3.5」を発表した。注目すべき設計思想は「統合」——従来は別々に提供していたチャット用Medium 3.1と推論特化Magistralを1つのモデルに集約し、リクエストごとに推論深度を調整可能（thinking effort configurable）にした。SWE-bench Verified 77.6%はDevstral 2やQwen3.5 397B MoEを上回りオープンウェイトで最高水準。Vibe CLIではGitHub・Slack連携のサンドボックス型非同期クラウドエージェントが利用可能になり、「コーディングボット」から「自律タスクエージェント」へと進化した。開発者ツールVibe（旧Mistral Codestral環境）がCursorやGitHub Copilotと本格競合する構図が明確になった。

---

## 📊 詳細レポート

![[2026-05-03_Mistral-Medium-35-128B.svg|1600]]

---

## 🔍 特記事項

> [!note] 「統合モデル」戦略の競合対比
> Qwen3.6・Kimi k2など中国モデルも「1モデルで推論オンオフ切替」路線を採用しており、業界全体に「専用推論モデル」から「推論内包統合モデル」へのシフトが起きている。OpenAIはo3をGPT-5に統合済み。MistralがEU拠点としてこの潮流に乗ったことで、差別化はアーキよりも「プライバシー・EU規制準拠」の文脈にシフトするかもしれない。

> [!note] 77.6%の解釈——Qwen3.6の35B-A3Bと比べて
> 同週にリリースされたQwen3.6-35B-A3B MoEがSWE-bench 73.4%（r/LocalLLaMA記事参照）、Medium 3.5が77.6%とリードしているが、128B Denseの方が計算コスト・メモリ要件が大きい。「同等タスクでQwen3.6をより少ないパラメータで超えているか」の効率比較はまだ不完全で、単純なスコア比較以上の文脈が必要。

> [!note] 価格設定への批判——HN議論の核心
> API価格 $1.50/$7.50/1M tokは、DeepSeek V4 Flash（$0.07/$0.28）比で20〜25倍。「オープンウェイトなのにAPIはプレミアム」という矛盾がHNで指摘された。自己ホスト組は4GPU（A100相当）で動かせるとMistralは主張するが、VRAM要件を満たすには少なくとも$30,000〜40,000のハードウェア投資が必要で「本当に民主的か」論争が続く。

> [!note] Vibe非同期エージェントの意義
> MistralがVibe CLIに「バックグラウンドで走り続けるクラウドエージェント」を統合したことは、AIコーディングツールが「補助→自律執行」へと移行する象徴的な一手。ユーザーは「PR作成を依頼して離席→戻ったら完成」というワークフローが現実になる。Devinとの差はMedium 3.5という独自モデルをバックエンドに持つ点で、モデル改善がそのままエージェント性能改善に直結する構造。

> [!note] 1年先の予測
> MistralはEU AI規制を追い風にするため「Gemini/GPTより信頼できる欧州AI」ポジションを強化中。EU AI Act 8月施行でプロプライエタリモデルの運用コストが増す中、オープンウェイトかつEU本社という組み合わせは企業顧客に響きやすい。2026年後半のMedium 4か次期Mistral Large系が本命で、Medium 3.5はそのテスト台という位置づけが大きい。

---

## 🔗 関連記事

- [[2026-04-30_Qwen36-Open-Coding-Frontier]]
- [[2026-05-03_Qwen36-27B-Thinking-Preservation]]
- [[2026-05-03_Mistral-HN-Pricing-Debate]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
