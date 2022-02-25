# How to use this template

Este template Docker Compose aprovisiona un contenedor Kong con una base de datos Postgres, además de un load-balancer nginx. Después de ejecutar el template, el load-balancer nginx será el punto de entrada a Kong.

Para ejecutar este template:

```shell
$ docker-compose up
```
Para escalar Kong (ej. a tres instencias) ejecute:

```shell
$ docker-compose scale kong=3
```
Kong estará disponible a través de la instancia `nginx-lb` en los puertos `8000` y `8001`. Puede personalizar el template con sus propias variables de entorno o configuración de almacén de datos.
