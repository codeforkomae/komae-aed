# 狛江市 AED マップ

狛江市の AED 設置場所を地図上に表示するウェブアプリケーションです。データは東京都オープンデータカタログサイトより取得しています。

## セットアップ

1. このリポジトリをクローンします
2. GitHub リポジトリの Settings > Secrets and variables > Actions に移動します
3. 新しいシークレットを追加します:
   - Name: `GOOGLE_MAPS_API_KEY`
   - Value: あなたの Google Maps JavaScript API キー

## Google Maps API キーの取得方法

1. [Google Cloud Console](https://console.cloud.google.com/) にアクセスします
2. 新しいプロジェクトを作成するか、既存のプロジェクトを選択します
3. Maps JavaScript API を有効化します
4. Credentials ページで API キーを作成します
5. API キーの制限を設定することを推奨します:
   - Application restrictions: HTTP referrers (web sites)
   - Website restrictions: あなたの GitHub Pages の URL (例: `https://<username>.github.io/komae-aed/*`)

## デプロイ

- `main` ブランチにプッシュすると、GitHub Actions により自動的に GitHub Pages にデプロイされます
- デプロイされた URL は GitHub リポジトリの Settings > Pages で確認できます

## データソース

AED の位置情報は以下のオープンデータを使用しています:

- [東京都オープンデータカタログサイト - 狛江市 AED 設置場所](https://www.opendata.metro.tokyo.lg.jp/komae/132195_aed.csv)

## ライセンス

このプロジェクトは MIT ライセンスの下で公開されています。
