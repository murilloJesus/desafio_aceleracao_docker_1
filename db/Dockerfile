#docker run -it --name mysql --rm -p 3306 -e MYSQL_DATABASE=laravel -e MYSQL_ROOT_PASSWORD=root -v $(pwd)/.docker/dbdata:/var/lib/mysql mysql:5.7.22 --innodb-use-native-aio=0
FROM mysql:5.7.22

ENV MYSQL_ROOT_PASSWORD=root
ENV MYSQL_DATABASE=laravel

WORKDIR /var/lib/mysql/

COPY dbdata/ .

EXPOSE 3306
