# zabbix-docker-example

For use this examples you need docker instaled in your computer and use swarm mode

## Start swarm mode

```bash
docker swarm init
```

## Create monitoring-network

```bash
docker network create --driver overlay monitoring-network
```

## Create a stack with your prefer version

### Zabbix 4.0

- Deploy stack

```bash
docker stack deploy -c docker-compose-zabbix40.yaml zabbix40
```

- Access URL

```bash
http://127.0.0.1
```

- Remove stack

```bash
docker stack rm zabbix40
```

### Zabbix 4.4

- Deploy stack

```bash
docker stack deploy -c docker-compose-zabbix44.yaml zabbix44
```

- Access URL

```bash
http://127.0.0.1
```

- Remove stack

```bash
docker stack rm zabbix44
```

### Zabbix 5.0

- Deploy stack

```bash
docker stack deploy -c docker-compose-zabbix50.yaml zabbix50
```

- Access URL

```bash
http://127.0.0.1:8081
```

- Remove stack

```bash
docker stack rm zabbix50
```

