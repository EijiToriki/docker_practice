FROM ubuntu:20.04

# 環境変数
## イメージ・コンテナ作成時どちらでも有効
## コンテナ内で動的に環境変数で処理を変えるときに有効
# ENV hello="Hello World"
# ENV hoge="HOGEHOGE"

# 任意の変数
## イメージ作成時のみ有効な一時的変数
## docker build するときに有効。コンテナ実行時には何の影響も与えない。
## docker file内で生きていれば十分な変数にはARGを使う
# ARG message
# RUN echo $message > message.txt

ARG message_arg="Message Arg"
ENV message_env="Message Env"

RUN echo $message_arg > message_arg.txt
RUN echo $message_env > message_env.txt

CMD ["bash"]