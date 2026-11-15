# このリポジトリについて(Claude Code 向け)

このリポジトリは、知識ベースの **テンプレート(原本)** です(`_data/kb.json` の `is_template` が `true`)。

- 作業の前に **KB_GUIDE.md** を読んでください。特に「3. ファイルの3つの分類」「4-2. テンプレートで作業しているとき」「6. テンプレートを直したときの確かめ方」。
- ここで直した **共通の部分**(`kb-engine.json` に載っているファイル)は、各 notes が `python3 notes.py update` で取りこみます。どの notes でもそのまま動くように、題材の名前(Discord など)を共通の部分に直接書かず、`_data/kb.json` から読むようにしてください。
- 共通の部分のファイルを足した・消したときは、`kb-engine.json` も直してください。
- `notes.py` を直したら、`python3 notes.py check` に加えて、試しの notes での `init` と `update --from` まで確かめてください(KB_GUIDE.md の「6.」)。
- 記事は見本(`docs/01-example.md`)だけを置きます。題材ごとの記事は各 notes に書きます。
- コミット・push は、ユーザーに頼まれたときだけ行ってください。
