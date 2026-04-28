---
date: 2026-04-23
category: ビジネス
source: OpenAI / Fortune / Axios
url: https://fortune.com/2026/04/23/openai-releases-gpt-5-5/
impact: 3
tags: [AI, OpenAI, GPT-5.5, Spud, ベンチマーク, コーディング, AGI, エージェント]
cssclasses:
  - hide-properties
  - ai-news
---

# 🚀 GPT-5.5「Spud」リリース——GPT-4.5以来初の完全再学習ベースモデル、Terminal-Bench 2.0で82.7%達成

> [!tip] TL;DR
> OpenAIが**GPT-5.5**（コードネーム"Spud"）を4月23日にリリース。GPT-4.5以来初の**完全再学習ベースモデル**であり、エージェント型コーディングベンチ**Terminal-Bench 2.0で82.7%**（Claude Opus 4.7: 69.4%、Gemini 3.1 Pro: 68.5%を大幅に凌駕）。ただしAPIプライスは**GPT-5.4の2倍**に跳ね上がった。

> [!info] 引用元
> - 🔗 **URL**: [OpenAI launches GPT-5.5 — Fortune](https://fortune.com/2026/04/23/openai-releases-gpt-5-5/)
> - 📅 **公開日**: 2026-04-23
> - 🏷️ **カテゴリ**: #ビジネス
> - ⭐ **インパクト**: ⭐⭐⭐

---

## 📝 概要

> [!abstract]
> OpenAIは2026年4月23日、コードネーム「Spud」と呼ばれていた**GPT-5.5**を正式リリースした。GPT-4.5以来初めての完全再学習ベースモデルであり、単なるファインチューニングではなく基盤アーキテクチャから鍛え直されている。エージェント型コーディング・コンピュータ操作・知識労働・初期的な科学研究といった長時間文脈推論が必要な領域で際立つ性能向上を示した。特にTerminal-Bench 2.0（複雑なコマンドライン作業を評価）では**82.7%**とSOTA、SWE-Bench Proでは**58.6%**、Expert-SWE（中央推定作業時間20時間の超長期コーディングタスク）では**73.1%**を達成した。APIプライスはinput $5/output $30（per M tokens）とGPT-5.4の2倍になったが、コーディングタスクでの**トークン効率が大幅改善**したとされ、総合コストは抑えられるとOpenAIは主張する。Plus・Pro・Business・Enterprise各ユーザーがChatGPTとCodexプラットフォームから利用可能。

---

## 📊 詳細レポート

![[2026-04-23_GPT-5-5-Spud-Release.svg|1600]]

---

## 🔍 特記事項

> [!note] Terminal-Bench 2.0が示す「エージェント時代」の新評価軸
> Terminal-Bench 2.0はSWE-benchの後継的なベンチマークで、単なるコード補完ではなく、計画→ツール呼び出し→反復修正のサイクルを含むエージェント的作業を評価する。82.7%という数値は、競合モデルとの差が特に顕著だ。Claude Opus 4.7（69.4%）・Gemini 3.1 Pro（68.5%）を13ポイント超上回っており、エージェントコーディング市場でOpenAIがポジションを奪い返した形となる。「ベンチを制する者がCodexサブスクを制する」構図が2026年のAI競争の主軸になりつつある。

> [!note] 「Spud＝ジャガイモ」という名前の意図
> Axios報道によればコードネームは"Spud"（英語でジャガイモ）。VentureBeatの見出しは「GPT-5.5 is here, and it's no potato（ダメなモデルじゃない）」とかけた。OpenAI内部では新モデルに食品名をつける文化があるが（例：Strawberry、Orion）、"Spud"は控えめな名前で期待値をわざと下げる戦術との見方もある。実際、発表の数日前に内部試験が流出し「期待外れ」との評価が先行していたが、ベンチ公開後に一転して市場の評価が逆転した。

> [!note] 価格倍増の背景：コスト削減の先にある「価値課金」モデル
> GPT-5.4の価格（input $2.5/output $15 per M tokens）と比べ、GPT-5.5はinput $5/output $30と実質2倍。OpenAIはトークン効率の改善でネットのコストは下がると主張するが、エンタープライズ顧客にとっては明確な値上げだ。Pro版（$30/$180 per M tokens）は特に高く、「高付加価値タスクへの集中化」という方向性を示している。AIサービスが「量より質・高価格帯」へシフトするトレンドはAnthropicのClaude Opus 4.7でも同様で、業界全体のプライシング哲学の転換が鮮明になっている。

> [!note] Claude Mythosとの比較：gatedモデル vs オープン展開
> 興味深いのはGPT-5.5がClaude Mythos Preview（限定パートナー向け）を一部ベンチで上回った点だ。Mythosは公開されていないため比較は限定的だが、Terminal-Bench 2.0でGPT-5.5（82.7%）がMythos（約80.1%）を僅差で上回ったと複数メディアが報じている。MythosがProject Glasswing経由の限定提供であるのに対し、GPT-5.5は一般ユーザーに開放されており、OpenAIの「オープン展開＋高収益化」戦略が鮮明だ。

> [!note] 半年後の予測：GPT-5.5 Proと「エージェント経済」
> 現在のGPT-5.5はベースモデルの公開であり、数ヶ月以内にo5-level思考モードを統合した「GPT-5.5 Thinking」ないし「GPT-5.5-o版」のリリースが予想される。Terminal-Bench 2.0が示すエージェント能力と思考連鎖を組み合わせれば、Expert-SWEスコアがさらに10〜15ポイント伸びる余地がある。これが実現すれば、20時間相当の人間作業を自律的に完了させるAIコーダーが現実に近づく。Codexエンタープライズの課金構造と合わせ、2026年下半期の「エージェント経済」規模が見えてくる。

---

## 🔗 関連記事

- [[2026-04-23_Anthropic-1T-Secondary-Valuation]]
- [[2026-04-20_OpenAI-GPT-5-4-Cyber]]
- [[2026-04-21_OpenAI-Codex-Enterprise]]
- [[2026-W17|📅 Week 17 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
