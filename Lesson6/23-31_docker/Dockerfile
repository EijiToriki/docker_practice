# ベースとなるイメージ
FROM ubuntu:20.04

# イメージを作成する際に実行するコマンド
RUN apt update
RUN apt install -y curl

# ディレクトリの内容をコピー
COPY . /app/

# 初期実行されるコマンド
CMD ["ls", "-la"]