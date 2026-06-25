# Tsugai

Tsugai（番）は、キーボード操作を中心にした2画面ファイラーです。

## ダウンロード

最新版は GitHub の [Releases](https://github.com/drunk-monkey-suiken/tsugai/releases) からダウンロードしてください。

環境に合わせて以下を選びます。

- Windows: `Tsugai-vX.Y.Z-win-x64.zip`
- macOS: `Tsugai-vX.Y.Z-macOS-universal.zip`

ZIP を展開して実行してください。

## 動作環境

### Windows 版

- Windows 11 x64
- Windows 10 はサポート中の Enterprise・LTSC・IoT 系を対象
- 配布形式: 自己完結 exe
- .NET ランタイムの別途インストールは不要です

初回起動時に Windows SmartScreen の確認が出る場合があります。

### macOS 版

- macOS 14 Sonoma 以降
- Universal アプリ（Apple Silicon / Intel）

初回起動時に Gatekeeper の確認が出る場合があります。

## 主な操作

| キー | 動作 |
|------|------|
| `Tab` / `←` `→` | 左右ペイン切替 |
| `↑` `↓` | カーソル移動 |
| `Enter` | 開く / フォルダに入る |
| `Backspace` / `delete` | 親フォルダへ |
| `Space` | マーク切替 |
| `C` / `M` | コピー / 移動 |
| `R` | 名前変更 |
| `Delete` / `⌘` + `delete` | 削除 |
| `F` | インクリメンタルサーチ |
| `G` | 中身検索（grep） |
| `F5` | アクティブペインを更新 |
| `Z` | 設定 |

## 中身検索（grep）

`G` でフォルダ以下を再帰検索できます。

- 結果から `Enter` で該当ファイルの場所へ移動
- `Shift` + `Enter` でエディタの該当行を開く
- `Space` で行表示 / ファイル表示を切替
- `Esc` で検索結果を閉じる

Windows 版は設定で ripgrep などの外部検索ツールを指定できます。未設定時は内蔵スキャナを使います。
macOS 版も設定で検索ツールを指定できます。未設定時は内蔵スキャナを使います。

## 設定ファイル

設定はユーザーフォルダ配下に保存されます。

```text
Windows: %APPDATA%\Tsugai\
macOS:   ~/Library/Application Support/Tsugai/
```

## ライセンス

Copyright (c) 2026 drunk-monkey-suiken.

本ソフトウェアの無断転載、再配布、改変、リバースエンジニアリングを禁止します。
