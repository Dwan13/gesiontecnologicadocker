# Openproject y nginx

## Integrantes

### Dwan Felipe Veloza Paez
### Ivan Rene Arevalo Rios

#### Paso 1
Descargamos la imagen con `docker pull openproject/community`

#### Paso 2
Creamos un arhivo docker-compose-yaml donde se incluye:
* los servicios que son openproject y nginx
* puertos
* volumenes

#### Paso 3
Creamos el contenedor mediante `docker-compose up`

#### Paso 4
Verificamos funcionalidad con: `localhost:8080`
