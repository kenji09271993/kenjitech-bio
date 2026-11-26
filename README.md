# Kenjitech Bio — Website

kenjitech.bio の公式サイト（1ページ・静的HTML）。

## GitHub Pages で公開する手順

1. リポジトリの **Settings → Pages** を開く
2. **Source** を「Deploy from a branch」、ブランチを `main` / `/(root)` にして保存
3. 数分後、`https://<ユーザー名>.github.io/kenjitech-bio/` で表示される

## 独自ドメイン（kenjitech.bio）をつなぐ

独自ドメインを使うときは、リポジトリ直下に `kenjitech.bio` と1行だけ書いた `CNAME` ファイルを置き、ドメイン管理画面で以下のDNSを追加する。

| 種類 | ホスト | 値 |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | `<ユーザー名>.github.io` |

反映後、Settings → Pages で **Enforce HTTPS** にチェックを入れる。

## 更新方法

`index.html` を編集して `main` に push すると自動で反映される。
