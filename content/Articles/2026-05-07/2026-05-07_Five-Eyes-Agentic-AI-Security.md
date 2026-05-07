---
date: 2026-05-07
category: ビジネス
source: The Register / CISA / CyberScoop
url: https://www.cisa.gov/resources-tools/resources/careful-adoption-agentic-ai-services
impact: 2
tags: [AI, セキュリティ, エージェントAI, Five Eyes, CISA, 規制, サイバーセキュリティ]
cssclasses:
  - hide-properties
  - ai-news
---

# 🛡️ Five Eyesが初のエージェントAIセキュリティガイダンス：**23リスク・100以上のベストプラクティス**を公開

> [!tip] TL;DR
> 米英加豪ニュージーランドの5カ国サイバー機関（Five Eyes）が**初の共同エージェントAIセキュリティガイダンス**（30ページ）を発表。"Careful Adoption of Agentic AI Services"と題し、**23のリスク分類と100以上のベストプラクティス**を提示。「エージェントAIは既存のセキュリティ脆弱性を増幅させる」と警告し、ゼロトラスト・最小権限の既存フレームワークへの統合を推奨。

> [!info] 引用元
> - 🔗 **URL**: [CISA Guidance](https://www.cisa.gov/resources-tools/resources/careful-adoption-agentic-ai-services)
> - 📅 **公開日**: 2026-05-01〜07
> - 🏷️ **カテゴリ**: #ビジネス
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> CISA・NSA（米）、ASD・ACSC（豪）、Cyber Centre（加）、NCSC（英・NZ）が連名で「エージェントAIの慎重な採用」ガイダンスを公開した。文書は**特権リスク・設計/設定リスク・行動リスク・構造リスク・サプライチェーンリスク**の5大カテゴリに23のリスクを分類。中核メッセージは「エージェントAI専用の全く新しいセキュリティ規律は不要で、既存のゼロトラスト・多層防御・最小権限の原則を適用せよ」。発行直後にThe Registerが「警告内容よりも実装負担の現実」として批判的論評を掲載し話題になった。

---

## 📊 詳細レポート

![[2026-05-07_Five-Eyes-Agentic-AI-Security.svg|1600]]

---

## 🔍 特記事項

> [!note] 「新しいセキュリティ規律は不要」の含意
> 当局が「既存フレームワークで対応可能」とした背景には、エンタープライズ向けAIエージェント展開をガイドラインの欠如で萎縮させないという政策的判断がある。ただし実務者からは「最小権限の適用はLLMの非決定論的行動と相性が悪い」という指摘があり、理論と実装の乖離は大きい。

> [!note] サプライチェーンリスクが新焦点
> 23リスクのうちサプライチェーンリスクの記述が最も拡充されたのは、2025年後半に相次いだAIエージェントのSDKポイズニング事件（LangChain・CrewAI関連）を踏まえたもの。MCP（Model Context Protocol）経由のツールコールが悪意あるサードパーティプラグインをトリガーするシナリオが具体例として挙げられている。

> [!note] 法的拘束力ゼロという限界
> Five Eyesのガイダンスは「推奨」であり規制ではない。EUのAI法・NISディレクティブのような強制力はなく、米国では連邦AI法が存在しない状況が続く。Gartnerは「このガイダンスがコンプライアンスの"床"として機能するのは欧州と国防省系調達のみ」と予測し、民間市場での浸透には懐疑的な見方が多い。

> [!note] Claude Mythosの文脈での意味
> CISAがこのガイダンスを発行した直後の時期は、Claude Mythos Previewが内部でサイバー攻撃能力の高さが判明したタイミングと重なる。Pentagon AI契約でAnthropicが排除された経緯も加味すると、「エージェントAIの攻撃的用途抑制」が暗黙の背景目的である可能性を複数のアナリストが指摘している。

> [!note] 半年先：APAC・日本への波及
> 日本のIPAとデジタル庁はFive Eyes文書を参照しながら独自ガイドラインを策定中。2026年度内（2027年3月まで）に政府調達向けAIエージェント安全要件を追加する方向で検討されており、IT予算の組み換えが発生する可能性が高い。

---

## 🔗 関連記事

- [[2026-05-06_CAISI-AI-Predeployment-Testing]]
- [[2026-05-04_AI-Assisted-Attacks-2026-THN]]
- [[2026-05-04_GitHub-CVE-2026-3854-RCE]]
- [[2026-W19|📅 Week 19 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
