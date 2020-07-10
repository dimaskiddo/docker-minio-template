# Docker MinIO Deployment Template

This repository contains example of deployment implementation docker and docker-compose for MinIO project. This example is using docker images from [dimaskiddo](https://hub.docker.com/r/dimaskiddo) docker hub repository.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Prequisites package:
* Docker (Application Containerization)
* Docker-Compose (Docker Orchestration Tools)

### Deployment for Development

Standard deployment:
* Clone this repository to your current directory, make sure it's empty
```
git clone -b master https://github.com/dimaskiddo/docker-minio-template.git .
```
* Start MinIO environment services
```
docker-compose up -d
```

Additional deployment:
* Check running services information
```
docker-compose ps
```

Stopping services:
* Stop all services
```
docker-compose stop
```
* Stop specific service
```
docker-compose stop <service_name>
```

Destroying services:
* Destroying services only
```
docker-compose down
```
* Destroying services and remove all images
```
docker-compose down --rmi all
```

### Accessing Services

* MinIO service will be available in
  - http request: http://localhost or http://127.0.0.1

### Accessing MinIO Service

You can access / connect to your MinIO cache with information below
* Web UI: ```http://localhost or http://127.0.0.1```
* Hostname: ```minio```
* Port: ```80 or 443```
* Access Key: ```as declared in environment file```
* Secret Key: ```as declared in environment file```

## Built With

* [Docker](https://www.docker.com/) - Application Containerization
* [Docker-Compose](https://docs.docker.com/compose/) - Docker Orchestration Tools

## Authors

* **Dimas Restu Hidayanto** - *Initial Work* - [DimasKiddo](https://github.com/dimaskiddo)

See also the list of [contributors](https://github.com/dimaskiddo/go-whatsapp-rest/contributors) who participated in this project