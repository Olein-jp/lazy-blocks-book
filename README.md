# Lazy Blocks で WordPress ブロックを作ろう（仮）

Lazy Blocks プラグインを使って、WordPress で利用できるブロックを作る方法を解説する書籍の執筆データ管理レポジトリです。

## 目次

### はじめに
- 主な対象とする読者
- 本書では扱わない内容
- なぜ本書を執筆しようと思ったのか
- 執筆するにあたり意識したこと
- 本書内容の動作確認環境
- サポートサイトについて
- お問い合わせについて

### Lazy Blocks プラグインについて
- 概要
- プラグインのインストール方法
- プロ版について

### Lazy Blocks 基礎
- カスタムブロックを作るかどうかの判断
  - 最近の WordPress は便利になっている
  - それでもカスタムブロックが必要になる理由
  - メリットとデメリット
- Lazy Blocks の基礎知識
  - メニュー紹介
  - テンプレート機能とロックオプション
  - エクスポートとインポート
- Lazy Blocks を使ったブロックの作り方
  - ウィザードを利用したブロック作成方法
  - ウィザードを利用しない作成方法
  - ブロック作成画面の紹介
  - ブロックをコードで管理する方法
  - 出力する方法について（HTML+Hundlebars/PHP/Theme Template）
  - ブロックに可能な設定内容について
- テンプレートファイルなどの管理について
  - Theme Template の活用
  - 子テーマでの管理
  - CSS/JS の適応方法
    - Pro版ではないので独自に読み込まないといけない
    - ブロックごとにスタイルを読み込む `wp_enqueue_block_style()` が使えるかどうか確認
    - でなければ一括で読み込むしかない

### コントロール活用の基礎
- コントロールの基礎知識
  - コントロールとは
  - 追加方法と配置のベストプラクティス
  - 出力時の注意点（エスケープ）`https://www.lazyblocks.com/docs/blocks-code/php/`
  - 設置場所について
  - 設定可能項目について（利用できない単語についても紹介）`https://www.lazyblocks.com/docs/blocks-controls/overview/`
- 各コントロールの解説 `https://www.lazyblocks.com/docs/blocks-controls/overview/`
  - Email
  - Number
  - Password
  - Range
  - Text
  - Textarea
  - URL
  - Classic Editor(WYSIWYG)
  - Code Editor
  - File
  - Gallery
  - Image
  - Rich Text(WYSIWYG)
  - Checkbox & Toggle
  - Radio
  - Select
  - Color Picker
  - Date Time Picker
  - Repeater

### InnerBlocks の使い方
- InnerBlocks とは
- InnerBlocks の使い方

### 実際に作ってみよう
- FAQブロック
- カード型レイアウトブロック
- お知らせ一覧表示ブロック

### カスタムフィールドとの連携方法
- カスタムフィールドはどう使うべきだろうか
- SAVE IN META の利用方法
- コアブロックとの接続実験

### フックの活用
- 利用できるフック一覧
- よく使うフックと実装例
  - `lazyblock/my-block/frontend_callback`
  - `lazyblock/my-block/editor_callback`
  - `lazyblock/my-block/frontend_allow_wrapper`
  - `lazyblock/my-block/allow_inner_blocks_wrapper`

### まとめ
- Lazy Blocks の可能性
- 長期運用時の注意点（WordPress/Gutenberg の変化に対応する方法）
- さらに学ぶためのステップ（React 開発への入口）
- 本書のまとめ