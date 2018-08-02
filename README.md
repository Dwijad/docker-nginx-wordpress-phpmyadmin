# docker-nginx-wordpress-phpmyadmin
Docker compose to host a single wordpress site using NGINX/MariaDB/phpMyAdmin

Download the zip file and extract it. 

To host your own site change to NGINX directory

$ cd nginx

Modify the "server_name" directive in the following file and save it.

$ vi tuxlab.org.in

...

...


server_name "yourdomain.tld";

...

...


Build the docker image

$ docker-compose build

Run it

$ docker-compose up -d

The wordpress installer will be available at http://yourdomain.tld

Choose-

Database Name as: projectdb

User Name: admin

Password: password (You can change the password in docker-compose.yml)

Database Host: projectdb



The phpmyAdmin at http://SERVER_IP:8183
