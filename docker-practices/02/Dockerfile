# レイヤー①：ベースOSとして alpine: 3.17 を使用
FROM alpine:3.17

# レイヤー②：ビルドに必要なパッケージをインストール
RUN apk add --no-cache make

# レイヤー③：アプリケーションコード（Makefile）をコピー
WORKDIR /usr/src/app
COPY Makefile .

# レイヤー④：Makefile のターゲットを実行
RUN make