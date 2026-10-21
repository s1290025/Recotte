# Recotte! | レコッテ！

本と感想を残す、シンプルな読書記録アプリです。ログイン不要・ビルド不要です。

## できること

- Google Booksでタイトル・著者・ISBNを検索して登録
- 手動での登録、タイトル・著者の修正
- 読みたい / 読書中 / 読了の管理
- 読了日・感想の記録、編集・削除
- 記録の検索・絞り込み
- JSONバックアップの書き出し・読み込み（既存記録に追加し、同一IDは確認後に上書き）

## GitHub Pages

リポジトリの **Settings → Pages → Build and deployment** で、以下を選択して Save します。

- Source: Deploy from a branch
- Branch: main
- Folder: / (root)

公開先: https://s1290025.github.io/Recotte/

## データ保存

記録は利用中のブラウザのlocalStorageに保存します。端末・ブラウザを変えても自動同期しません。サイトデータを削除すると記録も消えるため、定期的に「書き出し」でバックアップしてください。バックアップを別のブラウザで読み込むこともできます。

読書記録はGitHubに送信しません。書籍検索語はGoogle Booksへ送信し、表紙画像は外部サービスから読み込みます。検索APIが利用制限等で失敗した場合も手動登録は利用できます。

## ローカルで動かす

このディレクトリで `python -m http.server 8000` を実行して http://localhost:8000 を開きます。
