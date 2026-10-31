アルプス公園マレットゴルフ スコアアプリ（アプリ化用ファイル）

ファイル
  index.html            アプリ本体（スコア表・マップ・ルール・アーカイブ）
  manifest.webmanifest  アプリ名・アイコンなどの設定
  sw.js                 オフラインで動かすための設定
  icon-192.png / icon-512.png / apple-touch-icon.png  アイコン

手順1: インターネット上に置く（GitHub Pages の例）
  1. github.com でアカウントを作り、新しいリポジトリを作る（Public）
  2. 「Add file」→「Upload files」で、このフォルダの6ファイルをすべてアップロードして Commit
  3. 「Settings」→「Pages」→ Branch を main / (root) にして Save
  4. 数分後に https://（ユーザー名）.github.io/（リポジトリ名）/ で開けるようになる

手順2-A: ホーム画面に追加（APKなしでアプリとして使う）
  Chrome で上のURLを開き、メニュー（︙）→「アプリをインストール」または「ホーム画面に追加」

手順2-B: APKにする
  1. https://www.pwabuilder.com/ を開き、上のURLを入力して Start
  2. 「Package for stores」→ Android を選び、Generate で zip をダウンロード
  3. zip 内の .apk を端末に入れてインストール（「提供元不明のアプリ」を許可）

データは端末のブラウザ内に保存されます。アプリを更新するときは sw.js の CACHE の番号を上げてください。
