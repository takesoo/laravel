# laravel
laravel開発環境(docker: php, nginx, mysql)

# 設定方法
## default.conf
default.conf => アプリ名.conf
```
server {
  listen 80;
    root /var/www/html/アプリ名/public;
    index index.php index.html;
```

## プロジェクト作成
docker-compose up -d

docker exec -it php bash

laravel new *project*

## DB接続設定
create database

.env変更
```
DB_CONNECTION=mysql
DB_HOST=db-host //DBコンテナ名
DB_PORT=3306
DB_DATABASE=dbname //DB名
DB_USERNAME=root //ユーザー
DB_PASSWORD= //パスワード
```

