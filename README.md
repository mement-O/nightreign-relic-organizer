# 🌙 Nightreign Relic Organizer

[🇯🇵 日本語](#-日本語) | [🇬🇧 English](#-english)

🌐 Web app: https://mement-o.github.io/nightreign-relic-organizer/

## 🇯🇵 日本語

ELDEN RING NIGHTREIGN の遺物整理を補助する非公式・読み取り専用ツールです。

セーブデータをブラウザ内で解析し、遺物の完全一致・上位互換・条件付き上位互換などを確認できます。不要マークや売却用表示、プリセット使用情報の表示、作業状態の JSON エクスポート / インポートにも対応しています。

### ✨ 主な特徴

- セーブデータはブラウザ内でのみ解析
- セーブデータへの書き込みは行いません
- 読み込んだセーブデータを外部サーバーへ送信しません
- JA / EN 表示切替
- 日本語名称・英語名称・EffectGroup を内蔵
- 完全一致 / 完全上位互換 / 上位互換 / 条件付き上位互換の確認
- 不要マークと売却作業用表示
- プリセット使用キャラクター表示
- 作業状態の JSON バックアップ / 復元

### 🖥️ 基本的な使い方

1. 上記の Web app を開きます。
2. `Import Save` から NIGHTREIGN のセーブデータを選択します。
3. 各タブで遺物を確認し、必要に応じて不要マークを付けます。
4. `売却用表示` を使ってゲーム内での売却作業を補助します。
5. 必要に応じて `Export State` で現在の作業状態を JSON に保存できます。

> 本ツールはセーブデータを直接編集しません。実際の売却操作はゲーム内で行ってください。

### 🔍 条件付き上位互換

このタブは、**使用者にとって不要な効果を指定し、その効果を「存在しないもの」として扱った場合に上位互換となる遺物がないかを探す**ための整理補助機能です。

例えば、ある遺物が次の3効果を持っているとします。

- 腐敗状態の敵に対する攻撃を強化＋2
- 凍傷状態の敵に対する攻撃を強化＋1
- 魔力攻撃力上昇＋4

このうち前2つを自分のビルドでは使わないと判断した場合、`無視する効果` でその2効果を選択します。すると本ツールは、それらを比較対象から除外し、残った `魔力攻撃力上昇＋4` を基準に、より良い候補が存在しないかをリストアップします。

この機能は「不要な効果が付いているから即売却」と判断するものではありません。**自分のプレイスタイルでは価値がない効果を除外して比較対象を広げ、手作業では見つけにくい整理候補を洗い出すための補助機能**です。

通常遺物は通常遺物同士、深層遺物は深層遺物同士で比較します。深層遺物のデメリット効果は、上位互換判定には使用しません。

### 🗑️ 売却用表示

`売却用表示` は、不要マークを付けた遺物を実際にゲーム内で売却するときの目視作業を補助する画面です。

本ツールはセーブデータを書き換えないため、不要マークを付けてもゲーム内の遺物は削除されません。**最終的な売却は、ゲーム内の遺物売却画面で利用者自身が行います。**

その作業をしやすくするため、売却用表示では次の点をゲーム内の売却画面に合わせています。

- 遺物の並び順
- グリッドの列構成
- 色
- 通常 / 深層の区別
- メリット効果数に応じたアイコンサイズ
- フィルタ適用後に対象外を詰める表示

不要マークを付けた遺物だけを強調表示できるため、**ツール側の一覧とゲーム内の売却画面を同じ並びで見比べながら、対象を順番に売却できます。**

さらに、売却対象が含まれる行だけを表示する機能や、前後の売却対象行へジャンプする機能も用意しています。

`プリセット使用（キャラクター名）` は注意表示として出ますが、ツール上では売却不可扱いにはしません。ゲーム内で実際に売却できるかどうかはゲーム側の状態に従ってください。

### 🔒 プライバシー / セキュリティ

セーブデータはブラウザ内でのみ処理されます。外部へのアップロード機能はありません。また、公開版 HTML では Content Security Policy によりネットワーク接続 API を禁止しています。

### 📚 参考情報

本ツールの実装・データ整理にあたり、以下のプロジェクト・情報源を参考にしています。

| Project / Source | 参考にした内容 |
| --- | --- |
| [alfizari/Elden-Ring-Nightreign-Save-Editor](https://github.com/alfizari/Elden-Ring-Nightreign-Save-Editor) | セーブデータ構造、遺物・効果パラメータ、日本語名称、Vessel / Preset 構造 |
| [metinc/nightreign-relic-browser](https://github.com/metinc/nightreign-relic-browser) | EffectGroup / level の整理 |
| [神攻略Wiki - 遺物効果](https://kamikouryaku.net/nightreign/?%E9%81%BA%E7%89%A9%E5%8A%B9%E6%9E%9C) | ゲーム内の遺物効果カテゴリ分類 |

これらのプロジェクト・情報源を参考にしていますが、Nightreign Relic Organizer は各プロジェクトの公式派生・共同開発プロジェクトではありません。

### ⚠️ 注意事項

本ツールは FromSoftware / Bandai Namco Entertainment の公式ツールではありません。

ゲーム本体から抽出した画像・音声等のリソースは同梱していません。参考元・Third-Party Notices・ライセンス情報は Web アプリ下部に記載しています。

---

## 🇬🇧 English

An unofficial, read-only relic organization assistant for ELDEN RING NIGHTREIGN.

The app analyzes save data locally in your browser and helps identify exact matches, outclassed relics, conditional upgrades, marked relics, sale targets, and preset usage. Work state can also be exported to and restored from JSON.

### ✨ Features

- Save data is processed only in your browser
- The app never writes to your save file
- Loaded save data is never uploaded to an external server
- JA / EN UI
- Embedded Japanese / English names and EffectGroup data
- Exact matches / strictly outclassed / outclassed / conditional outclassed checks
- Marked relics and sale-oriented view
- Preset usage indicators
- JSON work-state backup / restore

### 🖥️ Basic usage

1. Open the Web app linked above.
2. Use `Import Save` to select your NIGHTREIGN save file.
3. Review relics in each tab and mark unwanted relics as needed.
4. Use `Sale view` to assist with manual selling in-game.
5. Use `Export State` if you want to back up your current work state as JSON.

> This tool does not directly edit save data. Actual selling is performed manually in the game.

### 🔍 Conditional outclassed

This tab is intended to help find additional outclassed relics by letting you specify **effects that are irrelevant to your own build or playstyle** and temporarily treating those effects as if they did not exist during comparison.

For example, suppose a relic has these three effects:

- Increased attack against Scarlet Rot-afflicted enemies +2
- Increased attack against Frostbite-afflicted enemies +1
- Magic attack power up +4

If the first two effects are irrelevant to your build, select them under `Ignored effects`. The tool then excludes those effects from the comparison and searches for relics that outclass the remaining meaningful effect, `Magic attack power up +4`.

This does not mean that every relic containing an ignored effect should automatically be sold. The feature is a **sorting aid that broadens the comparison by removing effects you personally do not value, helping surface candidates that are difficult to spot manually.**

Normal relics are compared only with normal relics, and Deep Relics only with Deep Relics. Negative effects on Deep Relics are not used for the outclassed comparison.

### 🗑️ Sale view

`Sale view` is designed to make the final manual selling process in-game easier after you have marked unwanted relics in the tool.

Because this tool never edits your save data, marking a relic as unwanted does not remove it from the game. **The final sale must still be performed manually on the in-game relic selling screen.**

To make visual matching easier, Sale view mirrors the in-game selling screen as closely as possible, including:

- relic order
- grid column layout
- relic color
- normal / Deep Relic distinction
- icon size based on the number of positive effects
- compacted layout after filters are applied

Marked relics can be highlighted, allowing you to **compare the tool and the in-game selling screen in the same order and work through sale targets visually.**

There are also options to show only rows containing sale targets and to jump to the previous or next row containing a sale target.

`Preset use (character)` is shown as a warning indicator only. The tool does not treat preset use itself as unsellable; whether the relic can actually be sold is determined by the game.

### 🔒 Privacy / Security

Save data is processed only in the browser. There is no feature that uploads save data externally. The public HTML also uses Content Security Policy to block network connection APIs.

### 📚 References

The implementation and data organization of this tool were informed by the following projects and sources.

| Project / Source | Used as reference for |
| --- | --- |
| [alfizari/Elden-Ring-Nightreign-Save-Editor](https://github.com/alfizari/Elden-Ring-Nightreign-Save-Editor) | Save data structure, relic/effect parameters, Japanese names, Vessel / Preset structures |
| [metinc/nightreign-relic-browser](https://github.com/metinc/nightreign-relic-browser) | EffectGroup / level organization |
| [神攻略Wiki - Relic Effects](https://kamikouryaku.net/nightreign/?%E9%81%BA%E7%89%A9%E5%8A%B9%E6%9E%9C) | In-game relic effect category classification |

These projects and sources were used as references. Nightreign Relic Organizer is not an official derivative of, or jointly developed with, any of them.

### ⚠️ Disclaimer

This is an unofficial tool and is not affiliated with or endorsed by FromSoftware or Bandai Namco Entertainment.

No images, audio, or other resources extracted from the game are bundled with this project. References, third-party notices, and license information are listed at the bottom of the Web app.
