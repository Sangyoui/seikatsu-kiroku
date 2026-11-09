# 生活記録表（Web版）

送り先ごとにURLを分けています。

| URL | 送り先 | おくすり手帳の欄 |
|---|---|---|
| https://sangyoui.github.io/seikatsu-kiroku/healthcare/ | t-healthcare@sakurajyuji.jp | あり |
| https://sangyoui.github.io/seikatsu-kiroku/imushitsu/ | y-imushitsu@sanyo-shokai.co.jp | なし |
| https://sangyoui.github.io/seikatsu-kiroku/kanri-romu/ | kanri-romu@asmarq.co.jp | なし |

- 1週間分の生活リズム（睡眠・日中の活動・気分）を記録し、PDFにしてメール・LINE・その他のアプリで送るページです。
- PC・スマホのブラウザで開くだけで記入できます。アプリのインストールやログインは不要です。
- 3つの版の違いは、送り先と「おくすり手帳（任意）」の欄の有無だけです。端末に保存される記録も版ごとに分かれています。
- おくすり手帳の欄がある版（healthcare）では、おくすり手帳の写真やPDFを記録と一緒に送れます。それ以外の版では、おくすり手帳は面談前アンケートで受け取ります。

### 個人情報について

- 入力内容（おくすり手帳の写真を含む）は、記入する方の端末（ブラウザ）の中にだけ保存され、インターネット上には送信されません。
- このリポジトリには、記入用のページ（`healthcare/index.html`、`imushitsu/index.html`、`kanri-romu/index.html`）だけを置いています。**記入済みの記録（PDF・画像・Excel）は、このリポジトリに絶対にアップロードしないでください。**（このリポジトリは公開設定です）

### 更新のしかた

1. 更新したい版のフォルダ（`healthcare`・`imushitsu`・`kanri-romu`）を開く
2. 右上の「Add file」→「Upload files」で、新しい `index.html` をドラッグ
3. 「Commit changes」を押す（数分で同じURLに反映されます）

※ ZIPを展開してアップロードするときは、外側のフォルダではなく、中にある `healthcare`・`imushitsu`・`kanri-romu` のフォルダをドラッグしてください。

### 版ごとの設定（index.html 内）

各 `index.html` の冒頭付近にある設定だけが版ごとに違います。

| 設定 | 内容 |
|---|---|
| `DEFAULT_TO` | 送り先メールアドレス |
| `KEY` | 端末に保存するときの名前（版ごとに別にする） |
| `SHOW_MEDS` | おくすり手帳の欄を表示する（`true`）／しない（`false`） |
