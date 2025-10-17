# たくおのHP（GitHub Pages）

このリポジトリは、**VARジェネレーター** と **木こりゲーム** を公開するための GitHub Pages サイトです。  
アドセンス審査を意識した最小構成（固定ページ/ads.txt/サイトマップ等）を含みます。

## 1. ローカルでの準備
```bash
git init
git add .
git commit -m "Initial commit"
```

## 2. GitHub リポジトリ作成 & Push
1. GitHub 上で新規リポジトリを作成（例: `brotherinendroll.github.io`）
2. リモートを追加
```bash
git branch -M main
git remote add origin https://github.com/brotherinendroll/brotherinendroll.github.io.git
git push -u origin main
```

## 3. GitHub Pages を有効化
- Settings → Pages → **Branch: `main` / folder: `/ (root)`** を選択  
- 数分後、`https://brotherinendroll.github.io/` で公開されます

## 4. AdSense の設置
1. AdSense のサイト追加で、上記公開 URL を登録（サブパス型でも OK）
2. 審査コード（サイト全体に挿入するスクリプト）を `index.html` の `<!-- ADSENSE_GLOBAL_TAG -->` に貼り付け
3. 審査通過後、広告ユニットを作成し、表示したいページに配信コードを貼る
4. ルート直下の `ads.txt` の `pub-XXXXXXXXXXXXXXXXXXXXXXXX` をあなたの Publisher ID に置換

## 5. サイトマップと robots.txt
- `sitemap.xml` のドメイン `YOUR_GITHUB_PAGES_DOMAIN` をあなたの公開 URL に置換
- `robots.txt` の `Sitemap:` も同様に置換  
- 置換後、Search Console にサイトマップを送信するとインデックス促進になります

## 6. ページ構成
- `index.html` … ランディング（両コンテンツへの導線、広告タグの差し込み位置）
- `var-generator/` … VAR ジェネレーター一式（アップロード済みの内容）
- `kikori-game/` … 木こりゲーム一式（アップロード済みの内容）
- `about.html` / `privacy.html` / `contact.html` / `terms.html`
- `ads.txt` / `robots.txt` / `sitemap.xml` / `styles.css` / `.nojekyll`

## 7. よくある審査ポイント（簡易チェックリスト）
- ナビゲーションが分かりやすい（トップから各ページへ遷移できる）
- 独自性のあるコンテンツ（オリジナルのツール/ゲーム）
- プライバシーポリシー、運営者情報、お問い合わせの明記
- スマホ対応（レスポンシブ）
- 低品質/空ページを避ける、過度なポップアップやリダイレクト無し

---

最終更新: 2025-10-17
