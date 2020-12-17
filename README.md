# Team Maker Api Server
## 初期設定
- `cd {レポジトリのルートディレクトリ}`
- `docker-compose build`
- `docker-compose up -d`
- `docker exec -it tm-app composer install`
- `docker exec -it tm-app cp .env.example .env`
- `docker exec -it tm-app php artisan key:generate`