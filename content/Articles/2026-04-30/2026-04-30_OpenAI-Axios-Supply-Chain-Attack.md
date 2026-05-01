---
date: 2026-04-30
category: ビジネス
source: The Hacker News / BleepingComputer / OpenAI
url: https://thehackernews.com/2026/04/openai-revokes-macos-app-certificate.html
impact: 2
tags: [AI, セキュリティ, OpenAI, サプライチェーン攻撃, macOS, 北朝鮮, 証明書, Axios]
cssclasses:
  - hide-properties
  - ai-news
---

# 🔐 OpenAI Axiosサプライチェーン攻撃：北朝鮮起因のRATが証明書署名フローに侵入——macOS全ユーザーに更新要求

> [!tip] TL;DR
> 3月31日（UTC）に人気npmライブラリ「Axios」が侵害され、OpenAIのmacOSアプリの**コード署名ワークフロー**を汚染。RemoteAccessTrojan（RAT）が混入したバージョンがOpenAI内部システムを経由。OpenAIは**macOS証明書を緊急失効**し、**ChatGPT・Codex・Codex-cli・Atlasの全macOSアプリを再ビルド**。5月8日以降は旧版が使用不能になる。北朝鮮起因の攻撃と複数の調査が指摘。

> [!info] 引用元
> - 🔗 **URL**: [The Hacker News](https://thehackernews.com/2026/04/openai-revokes-macos-app-certificate.html)
> - 📅 **公開日**: 2026-04-30
> - 🏷️ **カテゴリ**: #ビジネス
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> 4月30日、OpenAIはmacOSアプリユーザー全員に5月8日までの強制更新を求める緊急通知を発出。原因は3月31日に発覚したAxios npmパッケージのサプライチェーン攻撃。悪意あるAxios v1.14.1が`plain-crypto-js`という隠れた依存パッケージをインストールし、Windows・macOS・Linux対応のRATを展開。OpenAIのCI/CDパイプラインがこのバージョンを取り込んだ結果、macOSアプリの**コード署名証明書**が侵害リスクに晒された。OpenAIはAppleと協力して旧証明書によって署名されたバイナリの公証を無効化し、サードパーティのフォレンジック企業を介して調査を実施。ユーザーデータへのアクセスや既存インストールへのマルウェア混入は確認されていないとしている。

---

## 📊 詳細レポート

![[2026-04-30_OpenAI-Axios-Supply-Chain-Attack.svg|1600]]

---

## 🔍 特記事項

> [!note] Axiosサプライチェーン攻撃の手口
> Axiosは月間ダウンロード数数億回のnpmライブラリで、企業・OSSを問わず広く使われる。攻撃者はv1.14.1として悪意あるバージョンをnpmに公開し、内部依存として`plain-crypto-js`（実態はRAT）を仕込んだ。GitHubのActionsワークフローが自動的に最新バージョンを取得する設定になっていたOpenAIが被害を受けた。同様の攻撃パターン（人気npmパッケージの乗っ取り）は2021年のua-parser-js、2022年のnode-ipc等で前例がある。

> [!note] 「北朝鮮起因」の根拠と意味
> BleepingComputer・RoboRhythmsなど複数の独立調査が北朝鮮のLazarusグループ（もしくは関連APT）による攻撃と指摘。GitHubのActionsワークフローを狙うCI/CDサプライチェーン攻撃は2024〜2026年に急増しており、AI企業のコード署名鍵や秘密鍵を標的にした攻撃が定型化している。CISAが2025年に警告したパターンと合致する。

> [!note] AI企業固有のセキュリティリスク
> OpenAIのCodex・Claude Code等、AIアシスタントがコードを生成・実行する環境では、サプライチェーン侵害は特に危険。生成されたコードがAIの名の下に信頼され、CI/CDに自動的に組み込まれるフローは攻撃者にとって理想的なベクター。「AIが書いたコードだから安全」という誤認が将来の攻撃を助長しうる。

> [!note] LMDeploy CVE-2026-33626との比較
> 4月27日に発覚したLMDeploy SSRF脆弱性（公開後12.5時間で実悪用）と合わせると、AI推論インフラへのサイバー攻撃が2026年に「定型化」していることが浮かび上がる。NVIDIA・Anthropic・Google Cloud等、AI基盤プロバイダーへのサプライチェーン攻撃が今後も継続すると見られる。

> [!note] 企業としての対応評価と残課題
> OpenAIの対応は「被害確認前に証明書を失効させる予防的措置」として適切。但し「ユーザーデータや既存インストールへの影響はない」という主張の独立検証は限定的。5月8日の強制更新切り替えは性急との声もあり、特に企業環境でのアプリ管理で問題が生じる可能性がある。npmの信頼モデル自体の脆弱性は今回の事案では解決していない。

---

## 🔗 関連記事

- [[2026-04-27_LMDeploy-CVE-2026-33626-SSRF]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
