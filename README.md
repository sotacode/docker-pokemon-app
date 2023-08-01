# Proyecto Pokemon Nest

## Descripción

Este proyecto es un ejemplo de una API basada en Nest.js que utiliza MongoDB como base de datos para almacenar información sobre Pokemon. El stack de Docker Compose incluye los servicios de MongoDB, MongoDB Express (una interfaz de administración web para MongoDB) y la aplicación de ejemplo Pokemon Nest.

## Requisitos

- Docker
- Docker Compose

## Instalación

1. Clona el repositorio.

    `git clone https://github.com/sotacode/docker-pokemon-app.git`


2. Entra en el directorio del proyecto.

    `cd docker-pokemon-app`

3. Copia el archivo `.env_template` y renómbralo a `.env`. Luego, edita las variables de entorno según tus necesidades. `cp .env_template .env`

## Uso

Para iniciar el entorno de desarrollo, ejecuta el siguiente comando:

    docker-compose up -d

Una vez que los servicios estén en ejecución, podrás acceder a las siguientes URLs:

- MongoDB Express: [http://localhost:8080](http://localhost:8080) (username: `MONGO_USERNAME`, password: `MONGO_PASSWORD`)
- Pokemon API: [http://localhost:3000](http://localhost:3000)

La API de Pokemon te permitirá interactuar con la base de datos MongoDB y obtener información sobre los diferentes Pokemon.
Para ver ejemplos de endpoints revisa la url: [klerith/pokemon-nest-app](https://hub.docker.com/r/klerith/pokemon-nest-app)

## Detener el ambiente

Para detener el entorno de desarrollo, ejecuta el siguiente comando:

    docker-compose down
