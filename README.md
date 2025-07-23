# StockMaster

Sistema CRUD para la gestión de stock de un negocio, basado en arquitectura MVC con PHP y MySQL.  
Incluye interfaz de administración con phpMyAdmin y configuración mediante variables de entorno (`.env`).

---

## 1. Clonación del repositorio

Clona el repositorio usando SSH:

```
git clone git@github.com:Yanina-Penayo/stockMaster.git
cd stockMaster
```

---

## 2. Crear red docker

docker network ls
docker network create stockMaster_net

---

## 3. Archivo .env 

```
PHP_PORT=7070
PHPMYADMIN_PORT=1905
MYSQL_SERVER=db
MYSQL_DATABASE=stock_master
MYSQL_ROOT_PASSWORD=Root123
MYSQL_USER=appuser
MYSQL_PASSWORD=App123

```
## 4. Construir el entorno y levantarlo

```
docker-compose up -d --build
```
verificar el estado del docker

```
docker ps
```
## 5. Acceso a la aplicación

Aplicación PHP (CRUD):
http://localhost:7070

phpMyAdmin:
http://localhost:1905
Usuario: root
Password: Root123
