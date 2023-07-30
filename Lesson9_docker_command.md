## docker コマンド
### ホストとコンテナのポートを紐づける
docker container run -p ホスト側のポート:コンテナ側のポート イメージ

### dockerネットワークの一覧
docker network ls

### ネットワークの詳細情報を表示
docker network inspect ネットワーク

### 新しいネットワークを作成
docker network create ネットワーク

### 指定したネットワークに接続したコンテナを起動
docker container run --network ネットワーク イメージ

### ネットワークを削除
docker network rm ネットワーク
