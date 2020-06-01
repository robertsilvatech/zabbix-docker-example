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

### Zabbix 5.0

- Change the branch

```bash
git checkout zabbix50
```

- Deploy stack

```bash
docker stack deploy -c docker-compose.yml zabbix50
```

- Access URL

```bash
http://127.0.0.1:8081
```

- Remove stack

```bash
docker stack rm zabbix50
```

