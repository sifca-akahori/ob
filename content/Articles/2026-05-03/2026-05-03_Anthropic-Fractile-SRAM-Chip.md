---
date: 2026-05-03
category: ビジネス
source: Tom's Hardware / The Tech Portal
url: https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropic-in-early-talks-to-buy-inference-chips-from-uk-startup-fractile
impact: 2
tags: [AI, Anthropic, チップ, 推論, ハードウェア, Fractile, SRAM, サプライチェーン]
cssclasses:
  - hide-properties
  - ai-news
---

# 🔬 Anthropic × Fractile：DRAM不要SRAMチップで推論コスト1/10を狙う秘密交渉

> [!tip] TL;DR
> Anthropicが英国スタートアップFractileと推論チップ供給の**初期交渉中**と複数メディアが報道。FractileのオンダイSRAMアーキは従来比**最大25x高速・1/10コスト**を謳い、ARR $300億に対して推論コストが重石になっているAnthropicの粗利問題を解決する可能性。チップ商用化は2027年以降の見込み。

> [!info] 引用元
> - 🔗 **URL**: [Tom's Hardware](https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropic-in-early-talks-to-buy-inference-chips-from-uk-startup-fractile)
> - 📅 **公開日**: 2026-05-03
> - 🏷️ **カテゴリ**: #ビジネス
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> AnthropicはNVIDIA・Google（TPU）・Amazon（Trainium）の3ルートに加え、英国スタートアップFractileを**第4の供給源**として開拓する初期交渉に入った。Fractileは2022年設立のオックスフォード発で、演算とメモリを同一ダイ上にSRAMとして集積する「コンピュート・イン・メモリ」設計を採用。外部DRAMへのデータ転送が推論時の最大ボトルネックであることを突いた設計で、主力モデルの推論スループットを最大25倍、コストを1/10に圧縮できると主張する。Anthropicの年間収益は2026年3月に$300億ARRを超えた一方、推論コストが粗利を圧迫しており、AMD・Celestial AIと並ぶサプライチェーン多様化の一手と見られる。

---

## 📊 詳細レポート

![[2026-05-03_Anthropic-Fractile-SRAM-Chip.svg|1600]]

---

## 🔍 特記事項

> [!note] なぜSRAMなのか——アーキテクチャの根本的優位
> LLM推論の電力・遅延の大半は「演算チップ⇔HBM/DRAM間のデータ往来」に起因する。FractileはこれをSRAMオンダイ統合で消滅させる発想で、学術的には「Processing-In-Memory（PIM）」と呼ばれる方向性の実装例。同様のアプローチはSambaNova・Groqも追うが、Fractileはモデルサイズに合わせたタイル分割設計で量産コストを抑えているとされる。

> [!note] Anthropicの粗利問題——ARR $300億でも「儲かっていない」構造
> 2025年末のARR $90億から2026年3月に$300億へ急拡大したが、Claudeの推論コストは売上に比例して増大し、業界筋では粗利率30〜40%台と試算される（SaaSとして低水準）。OpenAI・Googleは自社インフラ・専用チップを持つ分だけ有利な立場にあり、Anthropicがハードウェア垂直統合に踏み込む「必然性」が高まっている。

> [!note] 競合ベンダーへの戦略的インパクト
> NVIDIAは現在Anthropicの推論ワークロードの大半を担う最大サプライヤ。Fractile成功は直接的にH200/B200需要を削る可能性があり、NVDA株への潜在的ヘッジとして市場が注目する。一方でFractileのチップは2027年以降予定で「交渉カード」として機能しているだけの可能性もあり、実際の供給まで何年かかるかは不透明。

> [!note] 英国半導体エコシステムの文脈
> Fractileを含む英国半導体スタートアップへの米AI企業の接触は、英国政府の「AI行動計画」（2026年1月）と連動する。Armの設計基盤を生かしたエコシステムが欧州で台頭しつつあり、Deepmind・Wayveに続く第3の産業クラスターが英国に生まれつつある。

> [!note] 1〜2年後の分岐点
> ①Fractile量産成功→Anthropic粗利率改善・独立性強化 ②チップ遅延→NVIDIA依存継続・コスト問題悪化 ③Googleが同様チップ技術を内製→第三者スタートアップの存在意義が消失。2027年のFractileサンプル出荷が最初の分岐点。

---

## 🔗 関連記事

- [[2026-04-27_Google-40B-Anthropic-Investment]]
- [[2026-05-03_Pentagon-Anthropic-Exclusion]]
- [[2026-05-03_MCP-Linux-Foundation-Agentic-AI]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
