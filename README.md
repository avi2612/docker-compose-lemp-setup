# Docker Compose For LEMP Stack
This repository is based on v3 compose,it will install and setup Nginx, Php7.2, Mysql, phpmyadmin 

1. Put your website data in "app" directory and configure sql connection properly
2. "db-data" directory is mounted to database container /var/lib/mysql path
3. "logs" directory is mounted to nginx webserver /var/log/nginx path
4. "db-dumps" directory will store mysql importing data

"phpmyadmin => ip_address:8080"

-------------------------------------------
.env file

 
   MYSQL_ROOT_PASSWORD=123456
   
   MYSQL_DATABASE=www_project
   
-------------------------------------------   
docker-compose up -d

docker-compose ps

### NOTE => MySQL port is mapped with host port 3306. So, can be accessible remotely, To secure this use any not common random port. 
