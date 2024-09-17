```sh
docker compose up -d
```
# Create topic

```sh
docker compose exec kafka kafka-topics --create --topic <topic_name> --partitions <num_partitions> --replication-factor <num_replication> --if-not-exists --bootstrap-server localhost:9092
```
# List all topic
```sh
docker compose exec kafka kafka-topics --list --bootstrap-server localhost:9092
```

# Remove Topic
```sh
docker compose exec kafka kafka-topics --delete --topic <topic_name> --bootstrap-server localhost:9092
```


# Describe Topic
```sh
docker compose exec kafka kafka-topics --describe --topic <topic_name> --bootstrap-server localhost:9092
```

# Information about Kafka brokers
```sh
docker compose exec kafka kafka-broker-api-versions --bootstrap-server localhost:9092
```


# Produce Message
```sh
# Send message
docker compose exec kafka kafka-console-producer --topic <topic_name> --bootstrap-server localhost:9092
```

# Consume Message
```sh
# Receive message
docker compose exec kafka kafka-console-consumer --topic <topic_name> --from-beginning --bootstrap-server localhost:9092
```

# Information Broker
```sh
docker compose exec kafka kafka-broker-api-versions --bootstrap-server localhost:9092
```

# Status of Cluster
```sh
docker compose exec kafka kafka-cluster --describe --bootstrap-server localhost:9092
```
