# s — schedule-poll 短縮URL

GitHub Pages の 404.html トリックを利用した短縮URLリダイレクタ。

## URL マッピング

| 短縮URL | リダイレクト先 |
|---|---|
| `tlab-utokyo.github.io/s/SLUG` | `GAS…/exec?action=poll&id=SLUG` |
| `tlab-utokyo.github.io/s/SLUG/results` | `GAS…/exec?action=results&id=SLUG` |
| `tlab-utokyo.github.io/s/SLUG/admin/TOKEN` | `GAS…/exec?action=admin&id=SLUG&token=TOKEN` |

## セットアップ

1. `404.html` 内の `GAS` 変数にデプロイURLを貼る
2. GitHub Pages を有効化（Settings → Pages → Branch: main）
