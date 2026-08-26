# Nightreign Relic Organizer

[日本語](#日本語) | [English](#english)

Web app: https://mement-o.github.io/nightreign-relic-organizer/

## 日本語

ELDEN RING NIGHTREIGN の遺物整理を補助する非公式・読み取り専用ツールです。

セーブデータをブラウザ内で解析し、遺物の完全一致・上位互換・条件付き上位互換などを確認できます。不要マークや売却用表示、プリセット使用情報の表示、作業状態の JSON エクスポート / インポートにも対応しています。

### 主な特徴

- セーブデータはブラウザ内でのみ解析
- セーブデータへの書き込みは行いません
- 読み込んだセーブデータを外部サーバーへ送信しません
- JA / EN 表示切替
- 日本語名称・英語名称・EffectGroup を内蔵
- 完全一致 / 完全上位互換 / 上位互換 / 条件付き上位互換の確認
- 不要マークと売却作業用表示
- プリセット使用キャラクター表示
- 作業状態の JSON バックアップ / 復元

### 使い方

1. 上記の Web app を開きます。
2. `Import Save` から NIGHTREIGN のセーブデータを選択します。
3. 各タブで遺物を確認し、必要に応じて不要マークを付けます。
4. `Sale view` / `売却用表示` を使ってゲーム内での売却作業を補助します。
5. 必要に応じて `Export State` で現在の作業状態を JSON に保存できます。

> 本ツールはセーブデータを直接編集しません。実際の売却操作はゲーム内で行ってください。

### プライバシー / セキュリティ

セーブデータはブラウザ内でのみ処理されます。外部へのアップロード機能はありません。また、公開版 HTML では Content Security Policy によりネットワーク接続 API を禁止しています。

### 注意事項

本ツールは FromSoftware / Bandai Namco Entertainment の公式ツールではありません。

ゲーム本体から抽出した画像・音声等のリソースは同梱していません。参考元・Third-Party Notices・ライセンス情報は Web アプリ下部に記載しています。

---

## English

An unofficial, read-only relic organization assistant for ELDEN RING NIGHTREIGN.

The app analyzes save data locally in your browser and helps identify exact matches, outclassed relics, conditional upgrades, marked relics, sale targets, and preset usage. Work state can also be exported to and restored from JSON.

### Features

- Save data is processed only in your browser
- The app never writes to your save file
- Loaded save data is never uploaded to an external server
- JA / EN UI
- Embedded Japanese / English names and EffectGroup data
- Exact matches / strictly outclassed / outclassed / conditional outclassed checks
- Marked relics and sale-oriented view
- Preset usage indicators
- JSON work-state backup / restore

### Usage

1. Open the Web app linked above.
2. Use `Import Save` to select your NIGHTREIGN save file.
3. Review relics in each tab and mark unwanted relics as needed.
4. Use `Sale view` to assist with manual selling in-game.
5. Use `Export State` if you want to back up your current work state as JSON.

> This tool does not directly edit save data. Actual selling is performed manually in the game.

### Privacy / Security

Save data is processed only in the browser. There is no feature that uploads save data externally. The public HTML also uses Content Security Policy to block network connection APIs.

### Disclaimer

This is an unofficial tool and is not affiliated with or endorsed by FromSoftware or Bandai Namco Entertainment.

No images, audio, or other resources extracted from the game are bundled with this project. References, third-party notices, and license information are listed at the bottom of the Web app.
