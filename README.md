# メダカ塾パークゴルフ Ver.1.8 静的公開ファイル

このフォルダの中身が、GitHub PagesまたはCloudflare Pagesへアップロードする完成ファイル一式です。

## GitHub Pages

1. このフォルダの中身をGitHubリポジトリの公開ルートへアップロード
2. GitHubのSettings → Pagesで公開元を設定
3. `index.html` があるブランチまたはGitHub Actionsを選択

`404.html` と `.nojekyll` を同梱しているため、GitHub Pagesのプロジェクトサイトでも画面内の移動と再読み込みに対応します。

## Cloudflare Pages

1. Cloudflare PagesでGitHubリポジトリを接続、またはこのフォルダをアップロード
2. ビルド設定を使う場合は、出力ディレクトリをこのフォルダに設定
3. `_redirects` により、画面内の移動と再読み込みに対応

## 保存方式

プレイヤー名、プレー日、スコア、メモ、履歴は利用者のブラウザLocalStorageに保存されます。
サーバー、データベース、ログインは使用しません。
ブラウザデータを消去した場合や別端末へ移行した場合は、CSV出力をバックアップとして利用してください。