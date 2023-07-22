## docker コマンド
### イメージをダウンロード
docker image pull イメージ名

### イメージ一覧を表示
docker image ls

### イメージを削除
docker image rm イメージ名

### コンテナを起動
docker container run イメージ名

### up状態のコンテナを一覧表示
docker container ls

### すべてのコンテナを一覧表示
docker container ls -a

### 起動中のコンテナを停止
docker container stop コンテナ名

### コンテナを再起動
docker container restart コンテナ名

### コンテナのログを確認
docker container logs コンテナ名

### コンテナを破棄
docker container rm コンテナ名

