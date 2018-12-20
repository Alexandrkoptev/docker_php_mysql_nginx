Nginx PHP Wordpress Mysql
1. Install requirements
- Git
- Docker
- Docker Compose 

2. Check Docker Compose compatibility file version 3.
- sudo docker --version
- https://docs.docker.com/compose/compose-file/


3. Image to use
- Wordpress:php7.2-fpm
- Nginx:latest
- Mysql:5.7

4. This project use the following resourse host mashine:
-  ports : 80
-  volume: /var/lib/mysql

5. Clone the project
- Git clone https://github.com/Alexandrkoptev/docker_php_mysql_nginx.git


6. Run the progect
- cd ./ docker_php_mysql_nginx-master
- chek variables in file .env.example
- rm .env.example .env
- sudo docker -compose up –build


7. Download unzip and copy wordpress in code folder
- download latest version wordpress https://wordpress.org/download/
- unpack installation package and copy files in folder ./code
- example: unzip wordpressXXXX.zip    cd ./wordpress   cp -R . ~/docker_php_mysql_nginx-master/code/

8. Install wordpress
- Run your browser and follow the link http://127.0.0.1  
- Install wordpress

