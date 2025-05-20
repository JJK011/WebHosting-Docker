**Hosting a website using Docker**

This project has gone through multiple iterations.

**1. Wordpress based Site (initial version)**

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

**2. Custon Static Site (second version)**

Removed wordpress and mariadb and added a custom website made with html/css served directly using nginx in a docker container. The website is saved in 'SampleWebsite-main' folder.

**3. Hugo-powered Static Site (Current version)**

Replaced hand-coded html/css with a HUGO static site generator, still served via nginx, and cloudflare tunnel.
