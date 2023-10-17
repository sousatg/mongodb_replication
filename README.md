# MongoDB Replica Set

## Run

```
docker-compose up -d
docker exec mongo1 ./scripts/rs-init.sh
```

## Connecting

```
mongodb://mongo1:27017,mongo2:27017/db?replicaSet=rs0
```

Configure DNS
```
sudo -- sh -c "echo 172.20.0.2 mongo1 >> /etc/hosts"
sudo -- sh -c "echo 172.20.0.3 mongo2 >> /etc/hosts"
```
