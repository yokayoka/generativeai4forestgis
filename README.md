# 森林管理のための生成AI × WebGIS 勉強会

2026年11月7日〜8日のハンズオンで作成した Web 地図を公開するリポジトリです。

公開サイト: https://yokayoka.github.io/generativeai4forestgis/

スマートフォンで公開サイトを開く場合は、次のQRコードを読み取ってください。

<a href="https://yokayoka.github.io/generativeai4forestgis/">
  <img src="assets/public-site-qr.png" alt="WebGIS公開サイト（参加者ページ一覧）を開くQRコード" width="240" height="240">
</a>

## 構成

- `index.html`: 成果物の一覧
- `participants/pNN/`: 参加者ごとの公開ページ(成果物を提出した参加者分)
- `tools/sync_from_drive.ps1`: Google Drive の作業フォルダーを反映するスクリプト

氏名やメールアドレスはこのリポジトリに置きません。ID と氏名の対応は運営が非公開で管理します。

## 反映の流れ

1. 参加者が Google Drive の自分のフォルダーに `index.html` などを置く
2. 運営が `tools/sync_from_drive.ps1` を実行する(`-DryRun` で確認のみ)
3. `main` に push されると GitHub Pages に公開される

Google Drive に置くだけでは自動公開されません。入口の `index.html` は各参加者フォルダーの直下に置いてください。同期スクリプトは `pNN_` で始まるフォルダーを処理するため、`p23_…`・`p24_…` も対象です。

## ライセンス

コードは [MIT License](LICENSE)、文書等は CC BY 4.0 です。
