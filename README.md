# drive-post-assets

TikTok の Content Posting API は、投稿する画像を **こちら側の公開URLから取りに来る**
（`PULL_FROM_URL`）方式しか受け付けない。そのための置き場。

- `images/YYYY-MM-DD/NN/` — 送信する画像。送信が終わったら古い日付から消える。
- `callback.html` — TikTok と連携するときに、認可コードを受け取って表示するだけのページ。
- `privacy.html` / `terms.html` — TikTok 開発者ポータルに登録する規約ページ。

中身は `~/drive-tiktok-poster` の `run.py publish` が自動で置き換える。手で触る必要はない。
