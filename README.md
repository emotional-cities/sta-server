# SensorThings API Server

This server is the [FROST](https://fraunhoferiosb.github.io/FROST-Server/deployment/docker.html) implementation of the [OGC Sensor Things API Standard](https://docs.ogc.org/is/18-088/18-088.html).

## Quick Setup

You will need `docker` and `docker-compose` installed in your system, in order to run this infrastructure. 

First create a `.env` file with the environment variables. For example:

```
POSTGRES_PASSWORD="CHANGEme"
POSTGRES_USER="postgres"
```

Then run:

```
docker-compose up -d
```

Access the server on:
http://localhost:8080/FROST-Server/

## Add Data

```
curl -X POST -H "Content-Type: application/json" -d @sample.json http://localhost:8080/FROST-Server/v1.1/Things
```

## License

This project is released under an [MIT License](./LICENSE)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)