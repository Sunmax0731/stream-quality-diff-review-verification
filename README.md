# 配信品質検品・差分レビュー・手動検証

音量、解像度、シーン差分、手動確認、対応状況を同じ検品ビューで扱う。

| 項目 | 内容 |
| --- | --- |
| Rank | 66 |
| Domain | OBSStreaming |
| Idea No. | 4 |
| Repository | stream-quality-diff-review-verification |
| 主な公開先 | GitHub Release / BOOTH |

## Implementation

- `src/product-profile.mjs`: プロダクト定義。
- `src/core.mjs`: 入力正規化とバッチ評価。
- `src/validators.mjs`: 必須項目と warning 項目の検査。
- `src/review-model.mjs`: UI/レビュー向けモデル。
- `src/report.mjs`: Markdown / HTML レポート生成。
- `src/cli.mjs`: CLI。

## Validation

`npm test` で代表シナリオ、QCDS、docs ZIP、文字化けを検証します。

## Strict QCDS Docs

- [Remote benchmark](docs/qcds-remote-benchmark.md)
- [Strict metrics](docs/qcds-strict-metrics.json)
- [Traceability matrix](docs/traceability-matrix.md)
- [Release evidence](docs/release-evidence.json)
