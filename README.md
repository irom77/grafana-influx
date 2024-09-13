# grafana-influx
compose of grafana with influx

###

```
docker exec -it influxdb influx
auth
buckets
```

.env
DOCKER_INFLUXDB_INIT_MODE=setup
DOCKER_INFLUXDB_INIT_USERNAME=myuser
DOCKER_INFLUXDB_INIT_PASSWORD=mypassword
DOCKER_INFLUXDB_INIT_ORG=myorg
DOCKER_INFLUXDB_INIT_BUCKET=mybucket
DOCKER_INFLUXDB_INIT_ADMIN_TOKEN=mytoken

### aider

Create docker compose file which will setup  `grafana` and `influx` database services to be used by grafana. Influx database service should read configuration parameters from .env file in `soar` subdirectory and setup database with name, user and password (or token if necessary) . Influx container should persist data.
Provide instructions to verify that influx database was created
