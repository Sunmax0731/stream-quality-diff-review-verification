# 要件定義

| 項目 | 内容 |
| --- | --- |
| Rank | 66 |
| Domain | OBSStreaming |
| Idea No. | 4 |
| Repository | stream-quality-diff-review-verification |
| 主な公開先 | GitHub Release / BOOTH |

## 背景

自動チェックと人の目視確認が分かれ、配信事故や対応漏れが起きやすい。

## 目的

音量、解像度、シーン差分、手動確認、対応状況を同じ検品ビューで扱う。

## 必須要件

- stream quality review を複数件まとめて検証できる。
- required fields: `id`, `title`, `baselinePath`, `currentPath`, `checklist`, `owner`。
- warning field: `manualFocus`。
- 代表シナリオ、QCDS metrics、docs ZIP、release evidence を再生成できる。
