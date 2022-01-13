<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Upute

Ako Docker nije instaliran kao sudo user ispred naredba za dockere treba dodati sudo!

1. Kreirati .env datoteku
2. Konfiguraciju za bazu:
 - DB_CONNECTION=mysql
 - DB_HOST=db
 - DB_PORT=3306
 - DB_DATABASE=db
 - DB_USERNAME=root
 - DB_PASSWORD=password
3. Kreirati Docker image od Laravel aplikacije:
 - docker build -t app .
4. Pokrenuti Docker-Compose instancu:
 - docker-compose up -d
5. Pokrenuti migraciju i seedanje unutar Laravel aplikacije:
 - sudo docker-compose exec app bash
 - php artisan migrate
 - php artisan db:seed   
