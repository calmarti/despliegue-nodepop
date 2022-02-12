# Configuración y despliegue en servidores

##  Ejercicio 1:
## Despliegue del backend de nodepop (node-express-mongodb)
IP-DNS:
```sh 
ec2-184-72-247-70.compute-1.amazonaws.com
``` 

## API
### Usuario por defecto
```sh
usuario: user@example.com
contraseña: 1234
```
### POST Autenticación
```sh
POST /apiv1/authenticate
```
### GET anuncios
Usar esta cabecera:
```sh
Header: x-access-token: <token>
```
```sh
GET /apiv1/anuncios
```
### POST anuncios
```sh
POST /apiv1/anuncios
```
Campos:
```sh
nombre, precio, venta, tags, foto
```

## Cabecera de origen de los ficheros estáticos
```sh
X-Owner: calmarti
```

## Ejercicio 2:
## Default server: frontend de nodepop (react)
```sh
184.72.247.70
```
El backend de la aplicación es el mismo usado en las prácticas de react (fundamentos y avanzado):

```sh
https://github.com/davidjj76/nodepop-api
```

La aplicación de react permite:

-Autenticarse en la aplicación con las credenciales:
```sh
usuario: user@user.com 
contraseña: 1234
```

-Filtrar los anuncios según nombre, venta/compra y tag, y sus combinaciones.

-Crear un anuncio nuevo 

-Borrar un anuncio 
