# Jenkins y Django

## Integrantes

### Dwan Felipe Veloza Paez
### Ivan Rene Arevalo Rios

#### Paso 1
Descargamos la imagen con `docker pull docker pull jenkins/jenkins`
#### Paso 2
Creamos un arhivo docker-compose-yaml donde se incluye:
`version: '2'
services:
  jenkins:
    image: 'jenkins/jenkins:lts'
    labels:
      kompose.service.type: nodeport
    ports:
      - '80:8080'
      - '443:8443'
      - '50000:50000'
    volumes:
      - 'jenkins_data:/jenkins_config'
volumes:
  jenkins_data:
    driver: local
`

#### Paso 3
Creamos el contenedor mediante `docker-compose up`

#### Paso 4
Verificamos funcionalidad con: `localhost:8080`
