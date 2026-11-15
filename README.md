# spring-boot-microservice-cloud-config

Configuration repository for the Spring Cloud Config server in [spring-boot-microservices-boilerplate](https://github.com/gillioa/spring-boot-microservices-boilerplate). It contains configuration only, no application code.

## Content
| Folder | Profiles | Notes |
|---|---|---|
| `api-gateway/` | `default`, `docker` | Port 8080, Eureka client, Hystrix settings |
| `discovery-service/` | `default`, `docker` | Eureka server settings |

Each profile is an `application.yml` file. The `default` profile points at `localhost`; the `docker` profile uses the docker-compose hostnames (`discovery-service`, `api-gateway`).

## Usage
The config-service of the boilerplate clones this repo over SSH (`git@github.com:gillioa/spring-boot-microservice-cloud-config.git`) and serves the files to the other services.

## Status
Archived, no further development planned.

## License
MIT