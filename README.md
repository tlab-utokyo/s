# schedule-poll Short URL Redirector

GitHub Pages の 404.html トリックを使った短縮 URL リダイレクタ。

## URL マッピング

| 短縮 URL | リダイレクト先 |
|---|---|
| `tlab-utokyo.github.io/s/SLUG` | `GAS?action=poll&id=SLUG` |
| `tlab-utokyo.github.io/s/SLUG/results` | `GAS?action=results&id=SLUG` |
| `tlab-utokyo.github.io/s/SLUG/admin/TOKEN` | `GAS?action=admin&id=SLUG&token=TOKEN` |

## セットアップ

1. `tlab-utokyo/s` リポジトリに `404.html`, `index.html`, `README.md` をアップロード
2. `404.html` 内の `YOUR_DEPLOY_ID` を実際の GAS デプロイ URL に書き換え
3. Settings → Pages → Branch: `main` → Save
4. 数分後に `https://tlab-utokyo.github.io/s/` が有効になる
