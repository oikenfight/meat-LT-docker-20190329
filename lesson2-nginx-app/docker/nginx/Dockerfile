FROM nginx:alpine

# ツールをインストール
RUN apk --no-cache update && \
    apk --no-cache upgrade && \
    apk --no-cache add \
    openssl

# ローカルに作成した設定ファイルをコンテナにコピー
COPY ./etc/nginx/conf.d/default.conf /etc/nginx/conf.d/default.conf
