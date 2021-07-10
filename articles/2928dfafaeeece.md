---
title: "DRYの原則"
emoji: "📑"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["アーキテクチャ"]
published: true
---

## 概要
Don't repeat yourself

直訳：同じコードを重複させるな。

本来の意図：ソフトウェア開発全体において情報を重複させない

DBスキーマ、テスト計画、ビルドシステムや、ドキュメンテーション等、幅広く適用できる。

この原則がうまく適用されたとき、いかなる変更も、関連のない要素の変更にはつながらない。さらに、関連する要素は統一的に変更され、それらの変更は同期が取れたものとなる。


## DRY 原則が有用でない場合
* 冗長化やミラーリング
* 構成管理
* 自動生成出力結果：生成コードで重複が排除されていれば良い。結果は重複していても良い。
* 過度なDRY：一つの関数が引数に応じて振る舞いを変化させる。

## 出典

[https://qiita.com/yatmsu/items/b4a84c4ae78fd67a364c:embed:cite]

[https://ja.wikipedia.org/wiki/Don%27t_repeat_yourself:embed:cite]

