# 蔵書管理ツール

個人の蔵書（漫画・書籍・雑誌）をブラウザだけで管理できるオフライン対応の単一HTMLファイルツールです。

https://reitovc.github.io/library/library_v4.html

## 特徴

- **インストール不要** — HTMLファイルをブラウザで開くだけで動作
- **オフライン対応** — データはすべてブラウザのIndexedDBにローカル保存
- **バーコードスキャン** — カメラまたは画像からISBNを読み取り、書誌情報を自動取得
- **シリーズ一括登録** — 巻数を選択してまとめて登録、ISBN自動取得に対応
- **複数ビュー** — 一覧・シリーズ・出版社の3種類の表示モード
- **CSV入出力** — データのエクスポート・インポートに対応

## 使い方

1. `library_v4.html` をダウンロード
2. ブラウザで開く（iPhoneの場合はNetlifyやGitHub PagesなどHTTPS環境を推奨）
3. 「＋ 登録」または「⚡ 高速登録」からバーコードスキャンで蔵書を追加

## 動作環境

- モダンブラウザ（Chrome / Safari / Firefox）
- IndexedDB対応（プライベートブラウジングモードでは動作しない場合があります）
- カメラスキャン機能はHTTPS環境が必要

## 技術スタック

- 単一HTMLファイル（依存ライブラリなし・オフライン動作）
- [PapaParse](https://www.papaparse.com/) — CSV処理
- [ZXing.js](https://github.com/zxing-js/library) — バーコード読み取り（初回スキャン時にlazyロード）
- IndexedDB — ローカルデータ保存
- openBD API — 書誌情報取得

## ライセンス

個人利用目的のプライベートツールです。
