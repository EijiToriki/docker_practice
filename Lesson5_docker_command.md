## docker コマンド
### docker run / exec のオプション
-i : 標準入力をオープンにする
-t : コマンドの見た目を綺麗にする
-d : バックグラウンド（デタッチ）モードで実行。常駐させたい処理がある場合に有効（例：nginxでhttpリクエストを待ち続ける場合）

### イメージの詳細情報を知る
docker image inspect イメージ名

- "Cmd" にデフォルトで実行されるコマンドが書かれている

### コンテナを起動して任意のコマンドを実行
docker container run -it イメージ名 任意のコマンド

- イメージからコンテナを新規作成して、コマンドを実行

### up状態のコンテナに任意のコマンドを実行
docker container exec コンテナ名 任意のコマンド

- 既存のコンテナでコマンドを実行する

### コンテナに任意の名前を付ける
docker container run --name 任意の名前

### Exitedのコンテナを一括削除
docker container prune

### コマンドの実行が終了したら直ちにそのコンテナを削除する
docker container run --rm イメージ名 任意のコマンド

- コンテナの使い捨てに有効

### up状態のコンテナであろうと矯正削除
docker container rm -f コンテナ名


### デタッチドモードになっているコマンドに接続
docker container attach コンテナ名

