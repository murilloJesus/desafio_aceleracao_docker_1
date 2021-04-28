# desafio_aceleracao_docker_1

para rodar a aplicação:

$ docker network create --driver bridge desafio_aceleracao_docker_1

$ docker run -it --name mysql --rm -p 3306:3306 --network desafio_aceleracao_docker_1 murillosjesus/mysql

$ docker run -it --network desafio_aceleracao_docker_1 -p 8000:8000 --name laravel --rm murillosjesus/laravel

$ docker run -p 8080:8080 --network desafio_aceleracao_docker_1  -it murillosjesus/nginx:latest


