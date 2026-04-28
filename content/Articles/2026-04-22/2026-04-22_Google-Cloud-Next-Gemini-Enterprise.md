---
date: 2026-04-22
category: 研究
source: Google Cloud
url: https://cloud.google.com/blog/products/ai-machine-learning/the-new-gemini-enterprise-one-platform-for-agent-development
tags: [AI, Google, GeminiEnterprise, A2A, エージェント, クラウド, マルチエージェント]
cssclasses:
  - hide-properties
  - ai-news
---

# 🌐 Google Cloud Next 2026：Vertex AI が「Gemini Enterprise Agent Platform」に刷新、A2A が本番150社へ

> [!tip] TL;DR
> Google Cloud Next 2026でVertex AIが**Gemini Enterprise Agent Platform**に改名・統合。エージェント間通信プロトコル**A2A**は150社が本番稼働に到達し、Salesforce・ServiceNow・SAP等との**カスタム統合コードゼロ**での相互運用を実現した。

> [!info] 引用元
> - 🔗 **URL**: [Google Cloud Blog — The new Gemini Enterprise](https://cloud.google.com/blog/products/ai-machine-learning/the-new-gemini-enterprise-one-platform-for-agent-development)
> - 📅 **公開日**: 2026-04-22
> - 🏷️ **カテゴリ**: #研究

---

## 📝 概要

> [!abstract]
> Googleは4月22日のCloud Next 2026基調講演で、AI開発プラットフォームの全面刷新を発表した。従来の「Vertex AI」は**Gemini Enterprise Agent Platform**に改称・統合され、ノーコードのエージェントビルダー、200以上のモデルカタログ（Anthropic Claudeを含む）、そしてエンタープライズ向けマネージドMCPサーバー群が一本化された。オープンプロトコル**A2A（Agent2Agent）**はLangGraph・CrewAI・LlamaIndex・Semantic Kernel・AutoGenへのネイティブ対応を追加し、本番稼働組織は150社に達した。Googleのエージェント専用Webブラウジングエージェント**Project Mariner**も同時に発表。Deloitteが専任のAgentic Transformation Practiceを立ち上げ、先行パートナーとなった。

---

## 📊 詳細レポート

![[2026-04-22_Google-Cloud-Next-Gemini-Enterprise.svg|1600]]

---

## 🔍 特記事項

> [!note] A2Aが「本番150社」の意味するもの
> A2Aプロトコルの150社本番稼働は、マルチエージェントオーケストレーションが「概念実証」から「インフラ標準」へ移行したことを示す最初の大規模証拠だ。Salesforceエージェント（Agentforce）とGoogle製エージェントが、カスタム統合コードなしにServiceNowのITアセットデータを照会できるという実例は、エンタープライズソフトウェア業界における「API時代からエージェント連携時代」への移行を象徴する。Microsoftのオープン仕様MCP（Model Context Protocol）が開発者寄りであるのに対し、A2AはSaaSベンダー間の業務連携に特化した設計思想を持つ。

> [!note] Vertex AI改名の戦略的含意
> Vertex AIという名称の廃止は、単なるブランド変更ではない。「AIモデルを使うプラットフォーム」から「AIエージェントを構築・運営する専用環境」へという製品コンセプトの転換を明示している。Googleはこれにより、OpenAIのCustom GPTs/Workspace Agents、AnthropicのClaude Platform/Coworkと同じ「エージェント構築プラットフォーム」市場で正面から激突する体制を整えた。200社以上のモデルラインアップにAnthropicのClaudeを含める点は、競合と協調が混在するコンペティティブ・コープ戦略の好例だ。

> [!note] Project Marinerとブラウジングエージェントの競争
> Googleが「Project Mariner」として提供するWebブラウジングエージェントは、OpenAIの「Operator」やAnthropicの「Claude in Chrome」と直接競合する領域に踏み込む。ブラウジングエージェントはRPA（Robotic Process Automation）の自然言語版として、バックオフィス自動化市場（年間推定600億ドル超）を侵食する可能性がある。GoogleはChrome・GWS・CloudのデータラインとProject Marinerを深く統合できる立場にあり、他社にはない垂直統合の優位性を持つ。

> [!note] Deloitteとの提携が示すコンサル市場の変容
> GoogleがDeloitteをAgentic Transformation Practiceの先行パートナーに据えた構図は、4月21日のOpenAI Codex LabsがCGI・Cognizantを取り込んだ動きと並行する。BIG4・大手SIer各社がAIプラットフォームベンダーと独自の認定・提携関係を結ぶ競争が加速しており、2026年末にはどのクラウドプラットフォームがコンサル経由の「実装標準」を握るかが、エンタープライズAI市場の版図を決定する重要変数となる。

> [!note] セキュリティレイヤー：Model Armor + ゼロトラスト
> A2Aのセキュリティ設計にはModel Armor（間接プロンプトインジェクション防御）・ゼロトラストアーキテクチャ・Cloud IAMによるアクセス管理と監査ログが組み込まれている。マルチエージェントシステムではエージェント間の信頼境界管理が最大の脆弱点となるため、この設計は重要だ。ただし「エージェントが別エージェントに権限を委譲する」ケースにおける最小権限原則の徹底度はまだ実運用での検証が必要であり、セキュリティコミュニティから注目を集めるだろう。

---

## 🔗 関連記事

- [[2026-04-22_Thinking-Machines-Lab-Google]]
- [[2026-04-22_Anthropic-Amazon-5GW-Compute]]
- [[2026-04-22_OpenAI-Workspace-Agents]]
- [[2026-W17|📅 Week 17 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
