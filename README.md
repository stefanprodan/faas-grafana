# faas-grafana

OpenFaaS Grafana [Docker image](https://hub.docker.com/r/stefanprodan/faas-grafana/)

Run Grafana in OpenFaaS Swarm network:

```bash
docker service create -d \
--name=func_grafana \
--publish=3000:3000 \
--network=func_functions \
stefanprodan/faas-grafana:4.6.3
```

URL: `http://<SWARM_IP>:3000/dashboard/db/openfaas`
