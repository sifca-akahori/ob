---
date: 2026-04-24
category: ビジネス
source: Tencent / Gigazine
url: https://gigazine.net/gsc_news/en/20260424-tencent-hy3/
impact: 2
tags: [AI, Tencent, Hy3, MoE, 中国AI, オープンソース, WeChat]
cssclasses:
  - hide-properties
  - ai-news
---

# 🐧 Tencent「Hy3 Preview」公開——295B-A21B MoEで推論効率+40%、WeChat/QQ即日統合

> [!tip] TL;DR
> Tencentが**元OpenAI研究者Yao Shunyu**率いる体制で開発したHunyuan Hy3 Previewを公開。**295B総パラメータ・21B活性・256Kコンテキスト**のMoEモデルで、前世代比推論効率 **+40%**。WeChat・QQ・Yuanbaoへ即日統合し、RMB **1.2元/Mトークン**（≒$0.17）という中国国内向け超低価格で展開している。

> [!info] 引用元
> - 🔗 **URL**: [Gigazine](https://gigazine.net/gsc_news/en/20260424-tencent-hy3/)
> - 📅 **公開日**: 2026-04-24
> - 🏷️ **カテゴリ**: #ビジネス
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> Tencentは2026年4月23〜24日にかけて、Hunyuanシリーズの刷新版「Hy3 Preview」をオープンソースとして公開した。アーキテクチャは「Fast-and-Slow Thinking Fused MoE」——高速なReactiveモードと低速なDeepThinkingモードを単一モデルに統合する設計で、295Bのうち21Bのみを各推論で活性化することで省電力と高性能を両立する。モデル重みはHugging Face・ModelScope・GitCodeで無料公開され、企業向けにはTencent Cloud TokenHubにて入力1.2元/M・出力4元/Mで提供。推論、指示追従、コーディング、エージェントタスクにおいて中国系トップモデルと肩を並べると主張しており、元OpenAI研究者の姚顺宇（Yao Shunyu）がリードした最初のフラッグシップとして注目されている。

---

## 📊 詳細レポート

![[2026-04-24_Tencent-Hy3-Preview.svg|1600]]

---

## 🔍 特記事項

> [!note] Yao Shunyu効果——OpenAI流RL知見の移植
> 姚顺宇は2024年まで OpenAIでRLHFおよびChain-of-Thought研究を担当していた人物。Hy3の「Fast-and-Slow」設計はOpenAIのo-seriesが確立した「Thinking Budget」概念の影響が色濃く、中国勢が米国ラボの知見を取り込むスピードが加速していることを示す。

> [!note] WeChat/QQへの即日統合がユーザー規模を即座にスケール
> Tencentが持つWeChatの月間アクティブユーザーは13億人超。Hy3はモデル公開と同時にWeChatのAIアシスタント「Yuanbao」に統合されており、単なるオープンソースリリースとは異なり、リリース翌日から数億人のエンドユーザーに触れる可能性がある。Llama系の学術ダウンロードとは桁違いの実世界スケールが論点となる。

> [!note] 「米勢に遅れ」という自己評価の意味
> Tencentのレポートは「米国フラッグシップ（GPT-5.5、Gemini 3.1-Pro）には及ばない」と認める。ただし中国市場向け価格（$0.17/M入力）とWeChatのディストリビューションを組み合わせると、性能より価格・統合性を優先する企業ユーザーには十分な選択肢となる。

> [!note] Alibaba Qwen 3.5との中国国内競争
> DeepSeek V4 Pro（同日公開）・Alibaba Qwen 3.5・Hy3 Previewが三つ巴で競合する構図になった。Alibaba は今月Tencent/Alibabaとして同時にDeepSeekへの出資を検討中（後述）であり、競争と協調が入り混じる複雑な中国AI勢力図が浮き彫りになっている。

> [!note] 半年後のシナリオ
> MoEの活性パラメータを21Bに抑えることで、スマートフォン（Snapdragon X Elite 等）への搭載が視野に入る。TencentがWeChatのデバイス上AI統合に踏み込めば、クラウド依存から端末推論への移行が加速し、「トークン課金ビジネス」自体を揺るがす可能性がある。

---

## 🔗 関連記事

- [[2026-04-24_DeepSeek-V4-Pro-Launch]]
- [[2026-04-24_DeepSeek-First-Funding-20B]]
- [[2026-W17|📅 Week 17 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
