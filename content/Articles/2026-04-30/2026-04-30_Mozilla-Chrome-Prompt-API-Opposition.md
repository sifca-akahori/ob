---
date: 2026-04-30
category: SNS
source: The Register / Hacker News / Mozilla
url: https://www.theregister.com/2026/04/30/mozilla_pushes_back_against_googles
impact: 2
tags: [AI, Google, Chrome, Mozilla, WebAPI, プライバシー, ブラウザ, 標準化]
cssclasses:
  - hide-properties
  - ai-news
---

# 🦊 Mozilla「Chrome Prompt API」に正式異議——HN 341pt・「Googleのウェブモノカルチャー」と業界論争

> [!tip] TL;DR
> MozillaがGoogleのChrome組み込みAI「**Prompt API**（window.ai）」に正式な反論を公開。「**ウェブの中立性・相互運用性・更新可能性に深刻な悪影響がある**」と指摘。HNで341ポイント・130コメントを集め「GoogleのNano LLMがウェブ標準のデフォルトになれば、Appleも取り込まれてモノカルチャー化する」との懸念が拡散。

> [!info] 引用元
> - 🔗 **URL**: [The Register](https://www.theregister.com/2026/04/30/mozilla_pushes_back_against_googles)
> - 📅 **公開日**: 2026-04-30
> - 🏷️ **カテゴリ**: #SNS
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> GoogleはChrome・Microsoft EdgeにAI推論層「Prompt API」を組み込み、ウェブ開発者が`window.ai`で直接LLM（Googleの「Nano」モデル）を呼び出せるようにしている。Mozillaはこれに対して「Prompt APIを通じてGoogleのNanoモデルが事実上の標準になり、開発者はNanoの動作・ToSに依存する。AppleとMozillaはNanoのライセンス取得を迫られるか、互換性が崩れるかの二択を迫られる」と批判。またPrompt API利用にはGoogleのGenerative AI Prohibited Uses Policyへの同意が必要であり、「法律違反ではない活動」も禁止されうる点を問題視した。同APIは現在ChromeとEdgeでテスト中。

---

## 📊 詳細レポート

![[2026-04-30_Mozilla-Chrome-Prompt-API-Opposition.svg|1600]]

---

## 🔍 特記事項

> [!note] Prompt APIが「ウェブ標準」になることの危険性
> W3CのWeb Platform仕様がベンダーニュートラルである理由は、標準を1社が支配しないためだ。Prompt APIがChrome/Edgeで動き、FirefoxとSafariで動かない、という現実が続けば、開発者は「Chrome前提」でAI機能を実装するようになる。これはかつてのInternet Explorer問題の現代版であり、ウェブ開発の多様性を根本から損なう。

> [!note] 「Prohibited Uses Policy」同意の問題
> Googleの生成AI禁止ポリシーは、法律上問題ない活動（例：競合製品のベンチマーク比較・政治的コンテンツ等）を禁止する可能性がある。ウェブAPIを通じて民間企業のポリシーへの同意が「標準」として組み込まれるのは前例のない構造で、EU DSA・AI Act的な観点からも問題になりうる。

> [!note] Apple・Firefoxはどう対応するか
> Chrome Engineerのコメント「懸念はもっともだ」という自認があるが、対策は示されていない。FirefoxはすでにAI機能のキルスイッチ追加を約束しており、Safariも独自のML推論（Core ML）をAPIとして提供する方向性がある。だが「相互運用性」の担保なく各社が独自実装を積み上げれば、かえってウェブのAI体験が断片化する。

> [!note] HNコミュニティの論点整理
> HN 130コメントの主な論点は3つ：(1) 「Googleがウェブ標準のチョークポイントを取ろうとしている」（政治批判）、(2) 「ローカルLLMのAPIが標準化されること自体は有益、ただしモデルは選択可能であるべき」（技術的折衷案）、(3) 「既にChromeのシェアが70%超なので事実上Googleが決める」（現実論）。いずれもGoogle側の応答次第で帰着が変わる。

> [!note] 業界への波及——AI Browser Standardsの闘争
> Prompt APIの議論は「ブラウザにAI推論を組み込む標準仕様」の主導権争いの序章に過ぎない。Mozilla/Appleが主体的に代替仕様を提案しなければ、デファクト標準はGoogleが握る。W3C AIコミュニティグループ（AIUG）の動向や、WHATWG側の対応が今後数ヶ月の分岐点になる。

---

## 🔗 関連記事

- [[2026-04-27_LMDeploy-CVE-2026-33626-SSRF]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
