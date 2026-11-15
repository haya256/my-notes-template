---
title: 記事の見本
nav_order: 1
summary: 記事の書き方の見本(notes.py init で消える)
keywords: [見本, サンプル, 書き方, frontmatter]
checked: 2026-11-15
verified: ネットのみ
thirdparty: []
source: (見本なので参考はなし)
---

# 記事の見本

## 要点

- これはテンプレートに置いている見本の記事です。`python3 notes.py init` で notes を始めると消えます
- 記事は `python3 notes.py new SLUG タイトル 説明` で作ります
- 書き方のルールは [KB_GUIDE.md](https://github.com/haya256/my-notes-template/blob/main/KB_GUIDE.md) の「8. 記事の書き方」にあります

## 手順

1. `python3 notes.py new voice-chat "ボイスチャンネルの使い方" "入り方と画面共有"` で記事を作る
2. 要点・手順・メモを書き、`keywords` と `source` を埋める
3. `python3 notes.py check` で確認する

## メモ

- 確かめていないことは「未確認」と書く。ネットの情報と、実機で確かめたことを分けて書く
- 実機で確かめたら `python3 notes.py verify docs/01-example.md 実機` で `verified` と `checked` を更新する
