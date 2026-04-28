---
date: 2026-04-23
category: SNS
source: Medium / Effloow / MCP Blog
url: https://medium.com/@claudio.a.lupi/mcp-just-hit-97-million-installs-7ca58aceff2f
impact: 2
tags: [AI, MCP, ModelContextProtocol, Anthropic, エージェント, インフラ, LinuxFoundation, 標準化]
cssclasses:
  - hide-properties
  - ai-news
---

# 🔌 MCP 9,700万インストール突破——16ヶ月でAIエージェント接続の「業界標準」に確立

> [!tip] TL;DR
> Anthropic発のModel Context Protocol（MCP）が2026年3月時点で**月間SDK9,700万ダウンロード**を達成し、AIインフラ標準として最速の普及曲線を記録。OpenAI・AWS・Microsoft・Google・Cloudflareら全主要プロバイダーが対応済みで、**1万以上の公開MCPサーバー**が稼働中。2025年12月にはLinux Foundationへ移管され、Anthropicの「標準」から業界の「共有インフラ」になった。

> [!info] 引用元
> - 🔗 **URL**: [MCP Just Hit 97 Million Installs — Medium](https://medium.com/@claudio.a.lupi/mcp-just-hit-97-million-installs-7ca58aceff2f)
> - 📅 **公開日**: 2026年4月（本週話題）
> - 🏷️ **カテゴリ**: #SNS
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> 2024年11月にAnthropicが公開したModel Context Protocol（MCP）は、2026年3月時点で月間SDK**9,700万ダウンロード**を記録した。ローンチ時（2024年11月）の200万から16ヶ月で約49倍に拡大した計算で、AIインフラ規格として史上最速の普及曲線だ。普及の転換点は2025年4月——OpenAIが自社製品・APIにMCPを採用したことで、「Anthropicの実験」から「業界標準」へと昇格した。その後AWSが2025年11月にネイティブMCPサポートを追加し、2025年12月にはAnthropicがMCPを**Linux Foundation**の傘下に新設された「Agentic AI Foundation」に移管（共同創設: Anthropic・Block・OpenAI、プラチナメンバー: Google・Microsoft・AWS・Cloudflare）。現在は**1万以上の公開MCPサーバー**が稼働し、主要SaaSツールとのAIエージェント連携が標準化されつつある。

---

## 📊 詳細レポート

![[2026-04-23_MCP-97M-Infrastructure-Standard.svg|1600]]

---

## 🔍 特記事項

> [!note] 「SQLみたいな存在になった」——プロダクションチームの生の声
> X/Twitterやmedium上のエンジニアレポートでは「MCPはAIエージェント開発の水道管になった」「ツール統合にMCPがなかった時代が思い出せない」という声が増えている。実際にプロダクション環境（6週間以上）でMCPを使っているチームからのレポートでは、Slackやデータベース、カレンダー等のSaaSとの接続が劇的に簡素化される一方、セキュリティ（サーバー乗っ取りリスク）とバージョン管理が主要な運用課題として浮上している。

> [!note] 9,700万→1億超を目前にした次の関門：エンタープライズセキュリティ
> Wiz Research（4月20日報道）によれば、MCP普及が1億5,000万インストールを突破した時点で「プロンプトインジェクション経由のサーバー乗っ取り」リスクが現実の脅威として浮上している。MCPサーバーが悪意あるコンテンツをモデルに注入することで、接続された全サービス（Slack・GitHub・カレンダー等）への不正アクセスが可能になる攻撃パターンが実証されている。Agentic AI Foundationがセキュリティ仕様の標準化を急ぐ必要がある。

> [!note] Linux Foundation移管が意味すること：「標準戦争の終戦」
> AWSがNetworkXを標準に、MSがODataを標準にしたように、AIツール接続の標準争いは実質的に終結した。Anthropicが自らMCPを「中立的な財団」に移管したことで、競合他社がより参加しやすくなり、標準としての持続性が高まった。この判断は短期的にAnthropicの「所有権」を失うが、長期的にはMCPエコシステムの規模拡大を通じてClaude・Claude Code製品の普及基盤を強化する戦略的合理性がある。

> [!note] 1万MCPサーバーの内訳と「ロングテール経済」
> 公開されている1万以上のMCPサーバーの大部分は個人・小規模開発者によるもので、Slack・Notion・GitHub・Jira・Linear・Figma等の主要SaaSへのコネクタが上位を占める。注目すべきは医療（EHR）・法務（判例データベース）・金融（Bloomberg API）という専門領域でのMCPサーバー開発が増加している点で、これらのニッチコネクタの累積がエンタープライズAIエージェントの「できること」を急速に拡張している。

> [!note] 半年後の予測：MCPの「モバイルアプリストア化」
> 現在はGitHubにセルフホスティングするスタイルが主流だが、半年以内にClaude.ai・Cowork・Codexなどのプラットフォームが「検証済みMCPサーバーマーケットプレイス」を提供し始めると予想される。これにより個人開発者がMCPサーバーをマネタイズできる市場が生まれ、「AIアプリストア経済」が形成される可能性がある。

---

## 🔗 関連記事

- [[2026-04-23_Stanford-AI-Index-2026]]
- [[2026-04-22_Google-Cloud-Next-Gemini-Enterprise]]
- [[2026-04-21_OpenAI-Codex-Enterprise]]
- [[2026-W17|📅 Week 17 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
