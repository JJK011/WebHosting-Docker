**Hosting a website built with Wordpress using Docker**

Website built on WordPress, MariaDB as database and nginx as webserver, hosted locally.

This locally hosted website is accessed from internet using cloudflare tunnel

**Docker images used**

Nginx

WordPress

MariaDB

Php:8-fpm

Cloudflared

**files**

docker-compose.yaml ----> Initializing various docker containers together

nginx_webserver_for_wordpress.conf ----> has the configuration for nginx to act as webserver for wordpress

cloudflare_token.env ---> has the token to access the cloudflare tunnel created in cloudflare website.
