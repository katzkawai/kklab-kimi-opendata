# kklab-kimi-opendata

ドル/円為替レートの長期時系列を可視化したオープンデータページです。

**公開ページ**: https://katzkawai.org/kklab-kimi-opendata/

## 概要

- IMF International Financial Statistics (IFS) のドル/円為替レート(月末、円/ドル)を取得し、Chart.js でインタラクティブな折れ線グラフとして公開しています
- 期間: 1957年1月〜2026年6月(月次、834件)
- 対数軸への切り替え、直近50年/30年/10年への期間絞り込みが可能です

## データ

- 出典: IMF IFS, 指標コード `ENDE_XDC_USD_RATE`(End of Period, 現地通貨/米ドル)
- `data/jpy_usd_monthly.csv` — 生データ(IMF API の出力そのまま)
- `data/jpy_usd_monthly.json` — グラフ描画用に整形したデータ

## ファイル構成

```
index.html                  可視化ページ(Chart.js)
data/jpy_usd_monthly.csv    為替レート生データ
data/jpy_usd_monthly.json   グラフ用データ
```

## 更新履歴

- 2026-08-08 グラフ下部に「為替変動に大きな影響を与えた主な出来事」の表を追加
- 2026-08-08 グラフのツールチップ表示を年月(YYYY-MM)形式に修正
- 2026-08-08 README を追加
- 2026-08-08 初版公開(ドル/円為替レート長期グラフ、1957年1月〜2026年6月)

## クレジット

このリポジトリは **Kimi K3** によって作成されました。
データの取得・加工・可視化ページの生成・GitHub Pages への公開まで、Kimi Code CLI 上で Kimi K3 が実施しています。

※ 本ページはデータ可視化を目的としたものであり、投資助言ではありません。
