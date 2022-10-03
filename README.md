## Oracle DB 18g - Docker

## Para iniciar la primera vez:

Pararse en la terminal en la carpeta oracle del proyecto

sudo docker-compose up -d

El contenedor actual crea una base llamada XEPDB1

El usuario de conexion es SYSTEM y la password es root

La url de conexion es: jdbc:oracle:thin:@localhost:1521/XEPDB1

-Luego de conectar se puede por consola crear un usuario de aplicación: crear_usuario.sql

-Luego también se puede conectar con ese usuario: dbuser y pass dbuser y crear tablas por ejemplo: crear_tablas.sql

## Siguientes veces:
Para stopear el contenedor:
sudo docker-compose stop

Para volver a levantalarlo:
sudo docker-compose start

## Comandos utiles de docker:

Para iniciar el docker:
sudo docker-compose up

Para iniciarlo en modo detach:
sudo docker-compose up -d

Para ver los contenedores creados:
sudo docker container ls -a / docker ps / docker ps -a

Para bajar y quitar un contenedor:
sudo docker-compose down

Para stopear un contenedor:
sudo docker-compose stop

Para borrar un contenedor o mas (primero hay que stopearlos):
sudo docker container rm {CONTANER_ID} {CONTANER_ID} {CONTANER_ID} ...

-Créditos para Gabriela Alcarraz por el Dockerfile base.-

