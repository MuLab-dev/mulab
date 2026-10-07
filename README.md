# Rakuly 公開ページ

App Store Connect に入力する「サポート URL」「プライバシーポリシー URL」用のページです。

| ファイル | 入力する欄 |
| --- | --- |
| `support.html` | サポート URL |
| `privacy.html` | プライバシーポリシー URL |
| `index.html` | マーケティング URL（任意） |

## 公開する前に

`【運営者名】` と `【メールアドレス】` を置き換えます（3つのファイルにあります）。ターミナルで、このフォルダに移動して：

```sh
sed -i '' -e 's/【運営者名】/あなたの名前や屋号/g' -e 's/【メールアドレス】/you@example.com/g' *.html
```

## GitHub Pages で公開する

1. GitHub で新しいリポジトリを作る（例：`rakuly`。Public）
2. このフォルダの中身（`index.html` `privacy.html` `support.html` `style.css`）をアップロードする
   （リポジトリの画面の「Add file」→「Upload files」でドラッグしても可）
3. リポジトリの「Settings」→「Pages」→ Branch を `main`、フォルダを `/ (root)` にして「Save」
4. 1〜2分で `https://<ユーザー名>.github.io/rakuly/` で開けるようになる
   - サポート URL：`https://<ユーザー名>.github.io/rakuly/support.html`
   - プライバシーポリシー URL：`https://<ユーザー名>.github.io/rakuly/privacy.html`

公開したら、iPhone のブラウザで3つとも開けることを確かめてから App Store Connect に入力します。
