# my-notes-template(知識ベースのテンプレート)

非公式の知識ベース(notes)を作るためのテンプレートです。
[my-discord-notes](https://github.com/haya256/my-discord-notes) のしくみを、題材を問わずに使えるようにしたものです。

- 記事はマークダウン。`verified`(実機で確認したか)や `checked`(確認日)などを記事ごとに管理する
- AI に読ませて質問に答えてもらうための「AIへの指示」付きの README
- GitHub Pages で読みやすいサイトになる(テーマは Just the Docs、日本語のサイト内検索に対応)
- 記事の管理スクリプト `notes.py`(Python 3 の標準機能だけで動く)
- **しくみ(共通の部分)はこのテンプレートで管理し、各 notes は `python3 notes.py update` で最新版を取りこむ**

## 新しい notes を作る

```bash
gh repo create my-slack-notes --template haya256/my-notes-template --public --clone
cd my-slack-notes
python3 notes.py init \
  --name my-slack-notes \
  --subject Slack \
  --owner-org "Slack Technologies" \
  --support-url https://slack.com/help \
  --github haya256/my-slack-notes
```

続きは [KB_GUIDE.md](KB_GUIDE.md) の「5. 新しい notes の作り方」を見てください。

## テンプレートの改善を notes に取りこむ

```bash
python3 notes.py update --diff
python3 notes.py check
```

## しくみと作業のルール

**[KB_GUIDE.md](KB_GUIDE.md) にすべて書いてあります。** テンプレートを直す人・AI も、notes で記事を書く人・AI も、作業の前に読んでください。

## ライセンス

テンプレートの文章とコードは [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.ja) で公開しています(著作権者:haya256)。
