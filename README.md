# GSCam Support Site (GitHub Pages)

GSCam（iPhoneアプリ）の **サポートページ / プライバシーポリシー** を GitHub Pages で公開するための静的サイトです。  
3言語（日本語 / English / 中文）に対応しています。

---

## 公開URL

GitHub Pages のURLは、通常以下の形式です：

- `https://<ユーザー名>.github.io/<リポジトリ名>/`

例：このリポジトリを `gscam-support` として公開した場合  
`https://<ユーザー名>.github.io/gscam-support/`

---

## ファイル構成（リポジトリ直下）

以下のファイルを **リポジトリ直下（root）** に配置してください。

### サポートページ
- `index.html`（English Support / トップ）
- `support-jp.html`（日本語 Support）
- `support-zh.html`（中文 Support）

### プライバシーポリシー
- `privacy.html`（English Privacy）
- `privacy-jp.html`（日本語 Privacy）
- `privacy-zh.html`（中文 Privacy）

> **重要**：もしローカル作業で `support-zh.generated.html` がある場合は、  
> **リポジトリに置くときはファイル名を `support-zh.html` にリネーム**してください。

---

## GitHub Pages の設定

1. GitHub リポジトリ → **Settings** → **Pages**
2. **Build and deployment**
   - Source：**Deploy from a branch**
   - Branch：`main`（または `master`）
   - Folder：`/(root)`
3. 保存（Save）

これで `index.html` がサイトのトップとして公開されます。

---

## 編集・更新手順

1. `index.html` / `support-jp.html` / `support-zh.html` などを編集
2. GitHub にコミット（commit）して push
3. GitHub Pages が自動更新されます

---

## ローカルで確認する（おすすめ）

macOS なら、フォルダに移動して簡易サーバーで確認できます。

```bash
cd <このリポジトリのフォルダ>
python3 -m http.server 8000
```

ブラウザで開く：

- http://localhost:8000/

---

## よくあるトラブル（キャッシュ）

### 変更したのに反映されない
多くは **ブラウザのキャッシュ** です。

- 強制リロード：`Cmd + Shift + R`（Mac / Chrome）
- さらに確実：DevTools を開いた状態でリロードボタン長押し →  
  **「キャッシュの消去とハード再読み込み」**

### それでも反映されない場合
- GitHub の **Actions** タブで Pages のデプロイが失敗していないか確認
- Pages の設定で公開元が `main / (root)` になっているか確認

---

## 言語切り替えとリンク

各ページ上部に言語切り替えリンクがあります：

- 日本語：`support-jp.html` / `privacy-jp.html`
- English：`index.html` / `privacy.html`
- 中文：`support-zh.html` / `privacy-zh.html`

---

## 連絡先

不具合報告・お問い合わせ：  
- ochiai@smartrig-app.com
