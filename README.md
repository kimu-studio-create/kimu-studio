# KIMU STUDIO — GitHub Pages 公開準備版

既存の「きむ本部」プラグインを変更せず、撮影指示を作成するスマホ向けWebアプリです。

## GitHub Pagesで公開する

1. GitHubにサインインし、新しい**Public**リポジトリ（例：`kimu-studio`）を作成する。
2. このZIPを解凍し、**中身**（`index.html`, `manifest.webmanifest`, `icon.svg`, `sw.js`, `.nojekyll`, `.github/workflows/deploy.yml`）をリポジトリのルートにアップロードして `main` ブランチへコミットする。隠しファイル `.github` と `.nojekyll` を忘れずに。
3. リポジトリの **Settings → Pages → Build and deployment → Source** を **GitHub Actions** にする。
4. **Actions** タブで `Deploy Kimu Studio to GitHub Pages` の実行が成功したら、**Settings → Pages** に表示されるURLを開く。通常は `https://<GitHubユーザー名>.github.io/kimu-studio/`。
5. iPhoneはSafariの共有メニューから「ホーム画面に追加」、AndroidはChromeのメニューから「ホーム画面に追加」を選ぶ。

## 現時点の機能・制約

- 撮影モード、背景、髪型、ポーズ、時間経過、衣装や髪の変化を選択し、撮影指示をコピーできます。
- 「きむ本部を開く」ボタンは既存プラグインのページへ移動します。**コピーした指示の貼り付け・送信は手動**です。
- 設定はその端末のブラウザ内に保存。JSON書き出し・読み込みに対応。**端末間同期・サーバー保存はありません**。
- 人物マスター画像は含まれません。**公開リポジトリに人物マスターや非公開情報をアップロードしないでください**。
- GitHub Pages公開はこのZIPを作った時点では未実施です。
- GitHub PagesのプロジェクトURL配下でも動く相対パス構成です。
