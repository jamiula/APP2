# APP2 Laravel demo project
For deploy this project please flow below guideline
1. Install docker and docker compose
2. git clone https://github.com/jamiula/APP2.git
3. cd APP2
4. cp .env.example .env
5. docker-compose build app
6. docker-compose up -d
7. docker-compose ps
8. docker-compose exec app ls -l
9. docker-compose exec app rm -rf vendor composer.lock
10. docker-compose exec app composer install
11. docker-compose exec app php artisan key:generate
12. docker-compose exec app php artisan cache:clear
13. docker-compose exec app php artisan route:clear
14. docker-compose exec app php artisan config:clear
15. docker-compose exec app php artisan view:clear
16. http://server_domain_or_IP:8001
