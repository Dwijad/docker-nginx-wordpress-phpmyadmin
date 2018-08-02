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

The wordpress site will be available at http://yourdomain.tld

The phpmyAdmin at http://SERVER_IP:8183
