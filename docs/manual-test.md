# 手動テスト

Codex側では手動テスト未実施です。

## 作業ディレクトリ

`D:/AI/OBSStreaming/stream-quality-diff-review-verification`

## 必要ファイル

- `dist/stream-quality-diff-review-verification-docs.zip`
- `docs/manual-test.md`
- `docs/strict-manual-test-addendum.md`
- `samples/representative-suite.json`

## セットアップ手順

```powershell
cd D:/AI/OBSStreaming/stream-quality-diff-review-verification
npm test
npm start
```

## ローカルサーバーやホストアプリ起動手順

OBS Studio を起動し、該当 scene/profile/log を手動確認する。現 closed alpha は CLI validation core を検証する。

## 実施手順

1. README と対象 Rank を確認。
2. 代表シナリオ4件を確認。
3. 生成 report を開く。
4. GitHub prerelease assets 3件を確認。

## 期待結果

error / warning / passed の意味が明確で、手順どおり再現できる。

## 未実施の手動確認項目

- 実ホストまたは実ブラウザでの継続利用確認。
- 公開先での表示確認。
- ユーザーによる S+ 昇格判断。
