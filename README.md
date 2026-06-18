# 納品書・請求書 PWA

スマホのホーム画面に追加して使える、納品書兼請求書作成アプリです。

## ファイル構成

```
invoice-pwa/
├── index.html       ← メインアプリ
├── manifest.json    ← PWA設定
├── sw.js            ← Service Worker（オフライン対応）
└── icons/
    ├── icon-192.png ← アプリアイコン
    └── icon-512.png ← アプリアイコン（大）
```

## 無料で公開する方法（GitHub Pages）

### 手順

1. **GitHubアカウント作成**（無料）
   - https://github.com にアクセスしてアカウント作成

2. **新しいリポジトリを作成**
   - 右上の「+」→「New repository」
   - Repository name: `invoice-app`（なんでもOK）
   - Public を選択
   - 「Create repository」をクリック

3. **ファイルをアップロード**
   - 「uploading an existing file」をクリック
   - このフォルダ内のファイルをすべてドラッグ＆ドロップ
   - 「Commit changes」をクリック

4. **GitHub Pagesを有効化**
   - リポジトリの「Settings」→「Pages」
   - Source: 「Deploy from a branch」
   - Branch: `main` / `/(root)` を選択
   - 「Save」をクリック

5. **URLが発行される**
   - `https://あなたのユーザー名.github.io/invoice-app/`
   - 数分後にアクセス可能になります

## スマホのホーム画面に追加

### iPhone (Safari)
1. Safariでアプリを開く
2. 下部の共有ボタン（四角に矢印）をタップ
3. 「ホーム画面に追加」→「追加」

### Android (Chrome)
1. ChromeでアプリのURLを開く
2. 右上の「⋮」→「ホーム画面に追加」
3. 「追加」をタップ

## 機能

- 請求情報・請求先・請求元の入力
- 明細（品名・数量・単位・単価・税率）の追加・削除
- 消費税（10%・8%・0%）の自動計算
- インボイス制度対応（登録番号入力）
- 振込先情報の入力
- **JSONファイルへの保存・読み込み**（編集途中のデータを保存可能）
- **PDFへの出力**（A4 1ページに収まるレイアウト）
- **オフライン動作**（一度開いたらネットなしでも使える）
- ダークモード対応
