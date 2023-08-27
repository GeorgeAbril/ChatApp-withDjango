# ChatApp  #

### Base de datos ###
Utiliza una base de datos simples a pesar que se solicito crear un atributo para almacenar
las ID de las conversación, actualmente solo guarda usuarios creados por consola.

## Pendientes ##
Este proyecto aún necesita mejoras como:

- Un registro de nuevos usuarios mediante interfaz 
- Agregar botones para redireccionar paginas
- Más pruebas
- Mejor documentación y comentarios
- Mejoras al fronted


1. Crear el espacio virtual en donde se ejecutara la App(siempre necesario)
```shell
pipenv --python 3 shell
```
2. Instalar los paquetes necesarios
```shell
pipenv install
```
3. Crear la base de datos en MySQL para que se conecte con el proyecto
```sql
CREATE DATABASE chat CHARACTER SET utf8;
```
4. Iniciar redis server en la PC
```shell
redis-server
```

5. Init la base de datos
```shell 
python manage.py migrate
```
6. Ejecutar tests de prueba
```shell
python manage.py test
```

7. Crear usuarios tipo Admin ya que no esta implentado el registro de usuarios aún
```shell
python manage.py createsuperuser
```

8. Levantar el servidor
```shell 
python manage.py runserver
```
