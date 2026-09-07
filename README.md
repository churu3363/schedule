# ベビの1日

赤ちゃんが起きた時間を起点に、ミルク・おむつ・家事・買い物・夜ルーティンを組み立てるWebアプリです。

## GitHub Pagesで公開する方法
1. GitHubで新しいRepositoryを作成
2. このZIPを解凍
3. 中のファイルを全部Repositoryの一番上にアップロード
4. GitHubの **Settings → Pages**
5. **Deploy from a branch** を選択
6. Branchを **main**、Folderを **/(root)** にして保存

## ホーム画面アイコンについて
このプロジェクトには `icon.png` を同梱していて、`index.html` に以下を設定済みです。
- favicon
- apple-touch-icon
- manifest.json

そのため、GitHub Pagesで公開したあとに **Safariでサイトを開いて「共有」→「ホーム画面に追加」** をすると、
この `icon.png` がホーム画面アイコンとして使われやすい構成になっています。

※ Shortcutsアプリで独自ショートカットを作る場合は、ショートカット側の仕様で手動アイコン設定になることがあります。
※ 一番自然にこのアイコンを使うなら、Safariからの「ホーム画面に追加」がおすすめです。

## データ保存
予定、メモ、チェック状態、追加したタスクはブラウザのlocalStorageに保存されます。
大事なデータはアプリ内の「バックアップ」でJSON保存しておくと安心です。
