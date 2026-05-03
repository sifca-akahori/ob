---
date: 2026-05-03
category: ビジネス
source: Anthropic / Linux Foundation
url: https://www.anthropic.com/news/donating-the-model-context-protocol-and-establishing-of-the-agentic-ai-foundation
impact: 2
tags: [AI, MCP, LinuxFoundation, AgenticAI, プロトコル, エコシステム, オープンソース, Anthropic]
cssclasses:
  - hide-properties
  - ai-news
---

# 🔌 MCP 97Mインストール突破・Linux Foundation Agentic AI Foundation：AI接続の「USB-C標準」が確立へ

> [!tip] TL;DR
> AnthropicのModel Context Protocol（MCP）が月次SDK**9,700万インストール**を突破。さらにAnthropicはMCPをLinux Foundation傘下の新組織「**Agentic AI Foundation（AAIF）**」に寄贈し、OpenAI・Block・AWS・Google・Microsoft・Cloudflareが共同ガバナンスに参加。Kubernetes・PyTorchと同じ「中立標準化」の道を歩み始めた16ヶ月間は、オープンソースプロトコル史上最速の採用曲線の一つ。

> [!info] 引用元
> - 🔗 **URL**: [Anthropic](https://www.anthropic.com/news/donating-the-model-context-protocol-and-establishing-of-the-agentic-ai-foundation)
> - 📅 **公開日**: 2025年12月（寄贈）/ 2026年3月（97M達成）/ 週末に最新解説が広く拡散
> - 🏷️ **カテゴリ**: #ビジネス
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> AnthropicはAIエージェントがツール・データソース・外部サービスと接続するための標準仕様「Model Context Protocol（MCP）」を、Linux Foundation傘下に新設された「Agentic AI Foundation（AAIF）」に移管した。共同創設者はAnthropic・Block・OpenAIで、AWS・Google・Microsoft・Cloudflare・Bloombergがプラチナメンバーとして参加。月次インストール数は2024年11月のローンチから16ヶ月で97Mに達し、主要AIプロバイダー全社がMCP互換ツールを出荷している状態になった。2026年MCPロードマップではSpec Enhancement Proposals（SEP）制度による標準進化・複数AIエージェント間の協調（マルチエージェントMCP）・セキュリティ強化レイヤーが予定されている。AI接続の「USB-C」ポジションを確固たるものにしつつある。

---

## 📊 詳細レポート

![[2026-05-03_MCP-Linux-Foundation-Agentic-AI.svg|1600]]

---

## 🔍 特記事項

> [!note] Kubernetes化戦略の含意
> AnthropicがMCPをLinux Foundationに寄贈したのは、Googleが2016年にKubernetesをCNCFに移管した戦略と同じ文法。「我々が作ったが、業界の標準にする」——これにより競合他社も参加しやすくなり、より大きなエコシステムが形成される。Anthropicは「MCPの親」としてのブランド価値を保ちつつ、標準策定の場では中立プレイヤーとして振る舞う。単一ベンダーへのロックイン懸念を払拭することで、エンタープライズ採用が加速する。

> [!note] 97Mインストールの地政学的意味
> 全主要AIプロバイダーがMCP互換ツールを出荷している状態は、「AIエージェントの接続方式でAnthropicが事実上の標準を作った」ことを意味する。これはAnthropicがモデル競争で1位でなくとも、「AIインフラの中心」に位置するという非常に強い立場を与える。APIエコノミーにおけるStripeやTwilioがそれぞれの分野で果たしたポジションに近い。

> [!note] マルチエージェントMCPが2026年の本命
> 2026年MCPロードマップの核心は「複数AIエージェントが互いをツールとして呼び出す」マルチエージェントプロトコルの標準化。A2A（Agent-to-Agent、Google I/O 2026で発表予定）との競合・補完関係が焦点で、どちらが「AIエージェント間通信の標準」になるかはエコシステム競争の最重要項目になる。

> [!note] セキュリティ強化の必要性——LMDeploy事件の教訓
> Week18に取り上げたLMDeploy CVE-2026-33626（公開13時間でSSRF悪用）のような攻撃が増える中、MCPサーバーがインターネットに露出する設計はサイバーリスクそのもの。AAIFのロードマップにはMCPレイヤーでの認証・認可・監査ログ標準化が含まれ、エンタープライズの実運用に必須の要件を埋める動きとして評価される。

> [!note] 日本企業へのインパクト
> 日本の主要ITベンダー（富士通・NTT・NEC等）もMCP互換ツールの開発に参入を表明しており、Cowork・ServiceNow・SAPなど業務システムとのMCP統合が2026年後半に本格化する見込み。LinuxFoundation参加により「オープン標準」として調達・セキュリティ審査が通りやすくなり、日本企業の採用ハードルが下がる。

---

## 🔗 関連記事

- [[2026-04-29_Enterprise-AI-Agent-Sprawl]]
- [[2026-05-03_Anthropic-Fractile-SRAM-Chip]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
