### Contenedor de Mysql

Este proyecto es una base para poder levantar un contenedor de mysql versión  *5.7* u *8*.

### Instrucciones

Lo primero que se debe hacer es copiar el archivo `.env.example` en un archivo `.env`, con el archivo generado, debemos completar la información de este:

```text
MYSQL_VERSION= <Versión de mysql puede ser 5.7 u 8>
PORT=<Puerto de salida en nuestra máquina>
NETWORK=<Red para que otros conenedores se puedan conectar>
CONTAINER_NAME=<Nombre del contenedor>
## Información para la conexión
DATABASE=
USER=
PASSWORD=
```

Con la información añadida desde la raíz de nuestro proyecto debemos ejecutar `docker-compose up -d` para levantar la base de datos. Con el contenedor corriendo podemos probar que la conexión es exitosa conectandonos a mysql desde nuestro gestor de base datos.