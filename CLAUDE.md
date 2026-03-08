# CLAUDE.md

このファイルは、Claude Code (claude.ai/code) がこのリポジトリで作業する際のガイダンスを提供します。

## 概要

日本語のスタンドアロン単一ファイルHTMLゲームのコレクション。各 `.html` ファイルはHTML・CSS・JavaScriptをすべて含む自己完結型のゲームです。ビルドシステム、パッケージマネージャー、テストフレームワークはありません。

## 実行方法

任意の `.html` ファイルをブラウザで直接開くだけで動作します。サーバーやビルド手順は不要です（依存ライブラリはすべてCDNから読み込まれます）。

## アーキテクチャ

各ゲームはインラインの `<style>` タグと `<script>` タグを持つ単一の `.html` ファイルです。CDNから読み込む2つの描画ライブラリのいずれかを使用しています：

- **Phaser 3**（2Dゲーム）: `2048.html`, `bb.html`, `rainbow_quest_rpg_phaser.html`, `snake2D.html`, `test.html`
- **Three.js**（3Dゲーム）: `baseball.html`, `chapter3_moon.html`, `floor-survival-fixed.html`, `kawaii-fps-survivor-v2.html`, `neko.html`, `srw.html`

## 基本ルール

- 応答・コメントはすべて日本語で行うこと

## デザイン規約

- 言語: UIテキストとコメントは日本語
- ビジュアルスタイル: 「Kawaii / ゆめかわいい」— パステルカラー（ピンク背景 `#FFF0F5` など）、丸みのある形状、ポップでドリーミーな世界観
- フォント: `M PLUS Rounded 1c`（Google Fonts）を標準書体として使用
- 対象プラットフォーム: モバイルファースト（ポートレート向き、タッチ操作）、`user-scalable=no` および `touch-action: none` を設定
