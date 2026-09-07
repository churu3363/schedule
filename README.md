# ベビの1日

赤ちゃんが起きた時間を起点に、ミルク・おむつ・家事・買い物・夜ルーティンを組み立てるシンプルなWebアプリです。

## GitHub Pagesで公開する方法

1. GitHubで新しいRepositoryを作成します。
2. このフォルダ内の `index.html`、`.nojekyll`、`README.md` をRepositoryの一番上にアップロードします。
3. Repositoryの **Settings** → **Pages** を開きます。
4. **Build and deployment** のSourceを **Deploy from a branch** にします。
5. Branchを `main`、Folderを `/ (root)` にして保存します。
6. 少しするとGitHub Pagesの公開URLが表示されます。

## データ保存について

日付ごとの予定、メモ、チェック状態、追加したタスクなどはブラウザの `localStorage` に保存されます。

そのため、
- 同じGitHub Pages URL・同じブラウザならデータは残ります。
- 別の端末や別ブラウザには自動同期されません。
- ブラウザデータを消すと保存内容が消える可能性があります。

アプリ内の **バックアップ** でJSONを書き出し、**復元** で戻せます。

## いまローカル版を使っている場合

GitHub Pagesに移すと保存先のURLが変わるため、ローカル版の `localStorage` は自動では引き継がれません。
移行前にローカル版でバックアップJSONを書き出し、GitHub Pages版を開いて復元してください。
