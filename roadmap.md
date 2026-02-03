# Rust学習ロードマップ

## Phase 1: Rust基礎 🌱

### 1.1 入門書で基礎固め

- [ ] [Rust入門](https://zenn.dev/mebiusbox/books/22d4c1ed9b0003) を完了
  - [ ] 環境構築（rustup, cargo）
  - [ ] 変数と型
  - [ ] 制御構文（if, loop, match）
  - [ ] 関数
  - [ ] 構造体（struct）と列挙型（enum）
  - [ ] 所有権（Ownership）の理解 ⭐重要
  - [ ] 借用（Borrowing）と参照の理解 ⭐重要
  - [ ] ライフタイム（Lifetime）の基礎 ⭐重要

### 1.2 公式ドキュメントで補強

- [ ] [The Rust Programming Language (TRPL)](https://doc.rust-lang.org/book/) の重要章を読む
  - [ ] Chapter 4: 所有権を理解する
  - [ ] Chapter 6: Enumとパターンマッチング
  - [ ] Chapter 8: 一般的なコレクション（Vec, String, HashMap）
  - [ ] Chapter 9: エラー処理（Result, Option）
  - [ ] Chapter 10: ジェネリクス、トレイト、ライフタイム

---

## Phase 2: Rust中級 🌿

### 2.1 より深い概念の理解

- [ ] トレイト（Traits）の深掘り
  - [ ] トレイト境界
  - [ ] 標準ライブラリの主要トレイト（Clone, Debug, Display, Iterator, From/Into）
- [ ] エラーハンドリングパターン
  - [ ] `?` 演算子の活用
  - [ ] カスタムエラー型
  - [ ] `anyhow` / `thiserror` クレートの理解
- [ ] クロージャとイテレータ
  - [ ] `map`, `filter`, `fold` などのイテレータアダプタ
  - [ ] クロージャのキャプチャと所有権

### 2.2 モジュールシステムとプロジェクト構成

- [ ] モジュール（mod）とファイル構成
- [ ] `Cargo.toml` の理解
- [ ] ワークスペース（複数クレート管理）の理解

---

## Phase 3: Rust実践 🌳

### 3.1 小さなプロジェクトで練習

- [ ] CLIツールを1つ作成する
  - [ ] `clap` クレートでコマンドライン引数処理
  - [ ] ファイル入出力
- [ ] [Rustlings](https://github.com/rust-lang/rustlings) で演習
- [ ] [Practice Rust](https://www.rustfinity.com/practice/rust/challenges) で問題を解く

### 3.2 テストとドキュメント

- [ ] ユニットテストの書き方
- [ ] 統合テストの書き方
- [ ] `cargo test` の使い方
- [ ] ドキュメントコメント（`///`）

---

## Phase 4: Biomeプロジェクトの理解 🔍

### 4.1 Biomeの概要を知る

- [ ] [Biome公式サイト](https://biomejs.dev/) を読む
- [ ] Biomeの機能を理解する（Linter, Formatter, etc.）
- [ ] Biomeを実際に使ってみる（自分のプロジェクトで試す）

### 4.2 開発環境のセットアップ

- [ ] [Biome リポジトリ](https://github.com/biomejs/biome) をFork & Clone
- [ ] [Contributing Guide](https://github.com/biomejs/biome/blob/main/CONTRIBUTING.md) を熟読
- [ ] ビルド環境を構築
- [ ] テストを実行してみる（`cargo test`）

### 4.3 ソースコード構造の理解

- [ ] ディレクトリ構造を把握
- [ ] 主要なクレートの役割を理解
  - [ ] `biome_parser`: パーサー
  - [ ] `biome_formatter`: フォーマッター
  - [ ] `biome_linter` / `biome_analyze`: リンター
  - [ ] `biome_cli`: CLIインターフェース
- [ ] 既存のPRを読んで変更パターンを学ぶ

---

## Phase 5: コントリビューション 🚀

### 5.1 コントリビューションの準備

- [ ] [Good First Issues](https://github.com/biomejs/biome/labels/good%20first%20issue) をチェック
- [ ] [Help Wanted Issues](https://github.com/biomejs/biome/labels/help%20wanted) をチェック
- [ ] Biome Discord / GitHub Discussions に参加

### 5.2 最初のコントリビューション

- [ ] 取り組むIssueを選択
- [ ] Issueにコメントして作業開始を宣言
- [ ] 実装
- [ ] テストを追加
- [ ] Pull Requestを作成
- [ ] コードレビューに対応
- [ ] **マージ完了！** 🎉

---

## 参考リソース 📚

### 書籍・チュートリアル

- [Rust入門 - Zenn](https://zenn.dev/mebiusbox/books/22d4c1ed9b0003)
- [The Rust Programming Language](https://doc.rust-lang.org/book/)
- [Rust By Example](https://doc.rust-lang.org/rust-by-example/)
- [もしもいま、Rustをイチから学び直すとしたら？](https://findy-code.io/engineer-lab/techtensei-matsu7874)

### 練習サイト

- [Rustlings](https://github.com/rust-lang/rustlings)
- [Practice Rust](https://www.rustfinity.com/practice/rust/challenges)
- [Exercism - Rust Track](https://exercism.org/tracks/rust)

### Biome関連

- [Biome 公式ドキュメント](https://biomejs.dev/)
- [Biome GitHub](https://github.com/biomejs/biome)
- [Biome Contributing Guide](https://github.com/biomejs/biome/blob/main/CONTRIBUTING.md)

---

## 学習のコツ 💡

1. **所有権・借用・ライフタイムは最重要**: コンパイラエラーと友達になろう
2. **毎日少しずつ**: 1日30分でも継続が大事
3. **実際に書く**: 読むだけでなく、手を動かす
4. **エラーメッセージを読む**: Rustのエラーメッセージは親切
5. **PHP/TSの知識を活かす**: 型システムや関数型の概念は転用できる

---

*最終更新: 2026-02-03*
