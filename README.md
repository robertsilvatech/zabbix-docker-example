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

### Zabbix 4.4

- Change the branch

```bash
git checkout zabbix44
```

- Deploy stack

```bash
docker stack deploy -c docker-compose.yml zabbix44
```

- Remove stack

```bash
docker stack rm zabbix44
```
