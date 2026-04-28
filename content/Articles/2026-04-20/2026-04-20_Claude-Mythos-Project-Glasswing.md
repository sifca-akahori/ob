---
date: 2026-04-20
category: 研究
source: Anthropic / NBC News
url: https://red.anthropic.com/2026/mythos-preview/
tags: [AI, LLM, Anthropic, セキュリティ, Mythos, Glasswing]
cssclasses:
  - hide-properties
  - ai-news
---

# 🛡️ Claude Mythos Preview と Project Glasswing 発表

> [!tip] TL;DR
> Anthropic が次世代モデル **Mythos** のプレビューを発表。脆弱性を「発見」だけでなく「武器化して実行」できるレベルに到達したため、**一般公開を見送り**、防御目的に限定した **Project Glasswing** として運用する判断を下した。

> [!info] 引用元
> - 🔗 **URL**: [Anthropic Red - Mythos Preview](https://red.anthropic.com/2026/mythos-preview/) / [NBC News](https://www.nbcnews.com/tech/security/anthropic-project-glasswing-mythos-preview-claude-gets-limited-release-rcna267234)
> - 📅 **公開日**: 2026-04-07
> - 🏷️ **カテゴリ**: #研究

---

## 📝 概要

> [!abstract]
> Anthropicは4月7日、新たな汎用言語モデル「Claude Mythos Preview」を発表した。全領域で高い性能を示す一方、コンピュータセキュリティ分野では **未発見脆弱性の特定＋武器化（weaponize）＋単独実行** を1モデルで完結できる水準に到達。この能力の二面性を受け、Anthropicは本モデルを一般公開せず、クリティカルソフトウェアの防御用途に限定した **Project Glasswing** として運用することを決定した。

---

## 📊 詳細レポート

![[2026-04-20_Claude-Mythos-Project-Glasswing.svg|1600]]

---

## 🔍 特記事項

> [!note] Anthropicが一般公開を見送った判断の重さ
> 過去にも高能力モデルのアクセス制限は存在したが、**「商用製品としてリリースしない」** という決断はAnthropicとしても異例。RSP（Responsible Scaling Policy）の想定する ASL-4 相当の能力判定が内部でなされた可能性が高く、業界他社（OpenAI・Google）がどう追随するかが注目される。

> [!note] Project Glasswingの実態
> 公開情報によれば、Glasswing はインフラ・金融・医療等のクリティカルソフトウェアを運用する **限定パートナー群** にのみ提供される。Mythosを「赤チーム」として使い、発見された脆弱性をAnthropicが責任ある開示プロセスに乗せる形。単なる研究プロジェクトではなく、**実運用の防御サービス** として設計されている点が新しい。

> [!note] AIセキュリティ能力の「非対称性」問題
> 攻撃AIと防御AIは同じ土台で動くため、能力ギャップが縮まると **「モデルを公開した瞬間に攻撃者が防御者と同等の力を得る」** という非対称性が顕在化する。Mythosの判断はこの問題への最初の具体的な応答と位置づけられる。今後、同等の能力を持つモデルはすべてGlasswing型の限定運用が検討されるようになる可能性がある。

> [!note] GPT-5.4-Cyberとの連動
> OpenAIが数日後に **GPT-5.4-Cyber** を発表したのは偶然ではない。Anthropicの限定公開判断が業界に与えた圧力の中、OpenAIは「防御特化派生モデル」という形で **公開可能な形に落とし込んで** リリース。両社の戦略の違いが浮き彫りになった週と言える。

> [!note] 今後の展開
> 業界観測筋は、Mythos本体の一般公開は **早くても6ヶ月以上先** と見る。それまでの期間、Anthropicは Glasswing 経由で蓄積した「攻撃→防御」の知見を、Claude Platform 全体の安全性レイヤーに還元する戦略と考えられる。2026年後半に向けて、AIラボの評価軸として「能力 × 責任ある展開」が主流になる兆しがある。

---

## 🔗 関連記事

- [[2026-04-20_Claude-Opus-4-7-GA]]
- [[2026-04-20_OpenAI-GPT-5-4-Cyber]]
- [[2026-W17|📅 Week 17 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
