# GitHub Pages 公開手順（経営指導員のためのプロンプト集）

## 含まれるファイル

| ファイル | 役割 |
|---|---|
| `index.html` | プロンプト集 Web 版本体（HTML 1ファイル・外部依存なし） |
| `経営・補助事業計画入力ガイド.pdf` | C1 持続化補助金プロンプトとセットで使う入力ガイド |

## 公開対象URL（例）

リポジトリ名を `keiei-shidoin-prompts` にした場合：
```
https://【GitHubユーザー名】.github.io/keiei-shidoin-prompts/
```

---

## 公開手順（所要時間：約10分）

### Step 1：GitHub にログイン
- https://github.com/ にアクセス
- 既存アカウントでログイン（なければ新規作成）

### Step 2：新規リポジトリ作成
1. 右上「＋」→ **New repository**
2. **Repository name**：`keiei-shidoin-prompts`（任意の名前でOK）
3. **Description**（任意）：例「商工会経営指導員のためのプロンプト集」
4. **Public** を選択（GitHub Pages 無料公開のため）
5. **Add a README file** にチェックを入れる
6. 「Create repository」をクリック

### Step 3：ファイルアップロード
1. リポジトリページで **Add file** → **Upload files**
2. このフォルダ（`_github_pages`）から **2ファイル** をドラッグ＆ドロップ
   - `index.html`
   - `経営・補助事業計画入力ガイド.pdf`
3. 下にスクロールし「**Commit changes**」をクリック

### Step 4：GitHub Pages を有効化
1. リポジトリトップ → **Settings**（右上）
2. 左サイドバー → **Pages**
3. **Source**：「Deploy from a branch」
4. **Branch**：`main` を選択、フォルダは `/ (root)`
5. **Save**

### Step 5：URL確認（数分待つ）
1. Settings → Pages を再度開く
2. ページ上部に「**Your site is live at https://〜**」と表示される
3. その URL をクリックして動作確認
4. PDF ダウンロード・コピーボタン・TOPボタンが全て動くか確認

---

## 検索エンジン非表示の確認

- HTML には既に `<meta name="robots" content="noindex, nofollow, ...">` を設定済み
- Google／Bing どちらも検索結果に出ません
- URL を共有した人だけがアクセス可能

---

## URL を共有する方法

1. **配布スライドにQRコード化して印刷**
   - QRコード作成サイト（例：https://qr.quel.jp/）に URL を貼る
   - PNG ダウンロード → 配布スライド／チラシに配置
2. **メールで案内**
   - 「研修参加者の皆さま限定 URL です」と添える
3. **当日のスライドに表示**
   - 最終スライドに URL と QR コードを掲載

---

## 更新方法（後日の改修時）

1. このフォルダで `index.html` を更新
2. GitHub リポジトリページ → `index.html` を選択 → 鉛筆アイコン（Edit）
3. または上書きアップロード（Upload files で同名ファイル）
4. **Commit changes**
5. 数分後に公開サイトに反映

---

## トラブルシューティング

- **「Your site is live」が表示されない** → 5〜10分待つ／ブラウザ更新
- **PDF がダウンロードできない** → ファイル名に日本語が含まれているため、ブラウザによってはエンコード警告が出ることがあります。動作は問題なし
- **誰かに見られたくない** → リポジトリを Private にすると GitHub Pages 無料公開は不可。Netlify／Cloudflare Pages の方が向きます

---

## 不明点があれば

鈴音（NAWAGATE 講習会ディレクター）までお気軽にお声がけください📖

最終更新：2026年5月28日
