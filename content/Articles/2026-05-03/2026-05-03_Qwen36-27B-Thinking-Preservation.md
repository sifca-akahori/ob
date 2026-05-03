---
date: 2026-05-03
category: 研究
source: Alibaba Qwen / Hugging Face
url: https://qwen.ai/blog?id=qwen3.6-27b
impact: 2
tags: [AI, Qwen, Alibaba, LLM, コーディング, オープンウェイト, Thinking, マルチターン, SWE-bench]
cssclasses:
  - hide-properties
  - ai-news
---

# 🧠 Qwen3.6-27B：27Bモデルが397B超えのコーディング性能、業界初「Thinking Preservation」

> [!tip] TL;DR
> AlibabaのQwen3.6-27Bが**SWE-bench Verified 77.2%**・Terminal-Bench 2.0で**Claude Opus 4.5と同スコア（59.3%）**を27Bパラメータで達成。最大の技術革新は「**Thinking Preservation**」——マルチターン会話で前の推論チェーンを次のターンに持ち越す業界初機能。Apache 2.0ライセンスで商用利用自由。週末にr/LocalLLaMAが沸騰。

> [!info] 引用元
> - 🔗 **URL**: [Qwen Blog](https://qwen.ai/blog?id=qwen3.6-27b)
> - 📅 **公開日**: 2026-04-22（週末に広く議論）
> - 🏷️ **カテゴリ**: #研究
> - ⭐ **インパクト**: ⭐⭐

---

## 📝 概要

> [!abstract]
> AlibabaのQwenチームがQwen3.6-27Bをリリースした。27BパラメータのDenseモデルでありながら、SWE-bench Verified 77.2%（Mistral Medium 3.5の77.6%に僅差）・Terminal-Bench 2.0 59.3%（Claude Opus 4.5同等）・QwenWebBench 1,487と、モデルサイズの常識を覆すスコアを記録した。262,144トークンのネイティブコンテキスト（最大101万トークンに延長可能）と、マルチモーダル対応（テキスト・画像・動画）も標準装備。最も注目すべき新機能は「Thinking Preservation」——通常、各ターンで思考プロセスが完全にリセットされるところを、このモデルは前ターンで行った推論チェーンを次のターンのコンテキストとして保持できる。長期的なコーディングセッションや複数ステップのデバッグにおいて、「前の思考を忘れない」AIエージェントが実現される。

---

## 📊 詳細レポート

![[2026-05-03_Qwen36-27B-Thinking-Preservation.svg|1600]]

---

## 🔍 特記事項

> [!note] Thinking Preservationの技術的意義
> 従来のLLMはマルチターン対話でも各ターンの「thinking tokens（推論中の内部トークン列）」がコンテキストウィンドウから消去されていた。Thinking Preservationはこれを保持し、「Turn 3の結論はTurn 1の推論Aに基づく」という依存関係を追跡できる。実装詳細は公開されていないが、思考チェーンの圧縮表現（abstracted CoT）をキャッシュする手法が有力視されている。長時間コーディングセッションで「なぜこのアーキを選んだか」をモデルが覚えているシナリオは実務上の価値が大きい。

> [!note] 27Bで397B超え——効率化の背景
> Qwen3.5 397B MoEを上回るスコアを27B Denseで達成した背景には、①蒸留によりより大きなモデルから知識を圧縮 ②合成データでコーディング特化訓練 ③KV-cacheの効率化でコンテキスト延長を実現——という3要素が重なっている。MoEはアクティブパラメータが少ないが推論インフラが複雑で、Dense小モデルの方が実運用では扱いやすいというトレードオフが見直されている。

> [!note] Apache 2.0が持つ戦略的意味
> Meta Llama 4がカスタムライセンスで商用利用に制限を設けて批判を受けた（Week18記事参照）直後に、QwenがApache 2.0で同等以上の性能を提供したことは、オープンソースコミュニティへの大きなシグナル。「Meta対抗・Llama代替」としての評価が一気に高まり、r/LocalLLaMAでは「Local AIのデファクトへ」という議論が起きている。

> [!note] Terminal-Bench 2.0の重要性
> SWE-bench Verifiedが「PRを解決できるか」を測るのに対し、Terminal-Bench 2.0は「3時間のタイムアウト内に32CPU/48GBRAMの環境で実際の端末タスクを自律執行できるか」を測る。より現実のエージェント利用に近い評価であり、27Bで Claude Opus 4.5と同スコアというのは「商用モデルを代替できる」という実用上の意味を持つ。コスト試算では推論費用を70〜80%削減できる可能性がある。

> [!note] 今後の展開——Qwen3-Coder-Nextが控える
> HuggingFace上ではすでに「Qwen3-Coder-Next」のプレースホルダが出現しており、コーディング特化の後継モデルが準備中と見られる。Qwen3.6-35B-A3B MoEとの組み合わせ戦略も含め、AlibabのオープンソースAI攻勢は2026年後半に最高潮を迎えると予想される。

---

## 🔗 関連記事

- [[2026-04-30_Qwen36-Open-Coding-Frontier]]
- [[2026-05-03_Mistral-Medium-35-128B]]
- [[2026-05-03_DeepSeek-V4-NIST-Evaluation]]
- [[2026-W18|📅 Week 18 サマリー]]

---
%% このノートは `ai-news-daily` タスクにより自動生成されました %%
