# Laravel lighthouse tutorial

Laravel lighthouseの学習用に下記を実行してみた
- Docker環境構築、高速化
- https://lighthouse-php.com/tutorial/
- https://www.toptal.com/graphql/laravel-graphql-server-tutorial

# 初期設定
1. `cd {レポジトリのルートディレクトリ}`
1. `docker-compose build`
1. `docker-compose up -d`
1. `docker exec -it lt-app composer install`
1. `docker exec -it lt-app cp .env.example .env`
1. `docker exec -it lt-app php artisan key:generate`
1. `docker exec -it lt-app php artisan migrate`

# 問題と対策
【問題】認証エラー発生時のResponseのエラー内容が理解しづらい

【対策】Lighthouseのエラーハンドリング処理を拡張して、エラー内容をわかりやすくした
 (参考) https://github.com/nuwave/lighthouse/issues/552#issuecomment-682118752
