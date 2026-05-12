---
date: 2026-05-12
category: 論文
source: Microsoft Security Blog
url: https://www.microsoft.com/en-us/security/blog/2026/05/07/prompts-become-shells-rce-vulnerabilities-ai-agent-frameworks/
impact: 2
tags: [AI, Microsoft, セキュリティ, RCE, AIエージェント, プロンプトインジェクション, LangChain, AutoGen]
cssclasses:
  - hide-properties
  - ai-news
---

# 🔐 Microsoft Security：「プロンプトがシェルになる」——主要AIエージェントフレームワークに RCE 脆弱性の連鎖を発見

> [!tip] TL;DR
> Microsoft Security Research（5/7）が主要AIエージェントフレームワーク（LangChain・AutoGen・CrewAI等）においてプロンプトインジェクションが**リモートコード実行（RCE）に連鎖する脆弱性クラス**を体系的に報告。「ツール呼び出しを許可したエージェントは、悪意ある入力に対してOSコマンド実行レベルの権限を与えている可能性がある」と警告。企業のAIエージェント展開に対し、インプットサニタイズの義務化を強く推奨している。

> [!info] 引用元
> - 🔗 **URL**: [Microsoft Security Blog — Prompts Become Shells](https://www.microsoft.com/en-us/security/blog/2026/05/07/prompts-become-shells-rce-vulnerabilities-ai-agent-frameworks/)
> - 📅 **公開日**: 2026-05-07
> - 🏷️ **カテゴリ**: #論文
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> Microsoftの研究チームは「Prompts Become Shells」と題した分析で、エージェントAIフレームワークの構造的なセキュリティ欠陥を指摘した。エージェントがシェルコマンド・ファイルI/O・外部APIを「ツール」として呼び出せる設計において、攻撃者がプロンプトに悪意ある指示を埋め込むことで、フレームワークが正規の処理として悪意あるコマンドを実行してしまう「プロンプトインジェクション→RCE」経路が確認された。特にLangChain の`exec`ツール、AutoGenの`code_execution_agent`、CrewAIのbashタスクが研究対象として挙げられた。同様の脆弱性は `github.com/openai/openai-agents-python`（OpenAI Agent SDK）でも確認されており、AIエージェント開発の主要ライブラリ全般に共通する設計上の脆弱性として位置づけられている。

---

## 📊 詳細レポート

![[2026-05-12_Microsoft-RCE-AI-Agent-Frameworks.svg|1600]]

---

## 🔍 特記事項

> [!note] なぜ今これが問題になるか——エージェント展開の急加速
> 2025年まではAIエージェントの「ツール呼び出し」は主にAPI呼び出し（天気検索・カレンダー追加等）にとどまっていたため、RCEリスクは限定的だった。しかし2026年には「コード生成→即実行」「シェルコマンド実行→結果フィードバック」というパターンが本番環境で広く使われ始めており、プロンプトインジェクション攻撃のリターンが格段に上がった。SAP Sapphire・Claude for Legalのような大規模エンタープライズ展開が進む中、この脆弱性クラスの修正は火急の課題になっている。

> [!note] 「インプットサニタイズ」の実装コスト——開発者の現実的な課題
> Webアプリ開発ではSQLインジェクション対策としてのパラメタライズドクエリが標準化されているが、自然言語プロンプトに対する「サニタイズ」は技術的に難しい。自然言語の意味的な多様性は固定的なブラックリストフィルタを容易に迂回でき、セマンティックな意図の判定には別のLLM（ガードレールモデル）が必要になる。これは「AIがAIを監視する」構造を生み、コストと複雑性が倍増するという現実的なジレンマを産む。

> [!note] フレームワーク各社の対応状況
> LangChainはv0.3.25で `allow_dangerous_deserialization` フラグのデフォルト変更による一部対策を実施済みだが、根本的なツール実行の権限分離は未実装。AutoGenはMicrosoft傘下であり、今回の研究と並行してMitigation PR（#4892）が提出されている。CrewAIはCVEの記録が相次いでいる状況で、独立系フレームワークの脆弱性対応サイクルの遅さが業界問題として浮上している。企業のAIエージェント展開でフレームワーク選定の際にセキュリティメンテナンス体制を評価する必要性が高まった。

> [!note] CISAとDoDの警告との接続
> 米国CISAと国防省は4月30日、「エージェントAIサービスの慎重な採用」に関するガイダンス文書を公開しており、今回のMicrosoftの発見はその技術的裏付けとなる。政府向けAI調達においてはこれらのフレームワーク使用に対し追加的なセキュリティ審査が課される可能性があり、公共部門でのエージェントAI展開に一定のブレーキがかかる可能性がある。

> [!note] 長期展望——「サンドボックスとしてのエージェントランタイム」の標準化
> 今後の解決策として有力視されているのは、エージェントの実行環境をDockerやWASMなどの軽量サンドボックスで完全隔離し、ツール呼び出しごとに権限を最小化するアーキテクチャだ。Google DeepMindのAgent Computer Interface（ACI）研究やAnthropicのコンピューターユース設計が参照点になっている。2027年にはOSI（Open Source Initiative）やNISTによる「安全なAIエージェントランタイム」標準仕様の策定が進む可能性があり、その標準に対応したフレームワークだけが企業採用に耐えうる地位を確立するだろう。

---

## 🔗 関連記事

- [[2026-05-12_AI-Agents-81pct-Autonomous-Hacking]]
- [[2026-05-11_Google-AI-Zero-Day-Attack-Blocked]]
- [[2026-05-11_SkillOS-Self-Evolving-LLM-Agents]]
- [[2026-W20|📅 Week 20 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
