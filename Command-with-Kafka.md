```sh
bash
```
# Create topic

```sh
/usr/local/kafka/bin/kafka-topics.sh --create --topic <topic-name> --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1

```
# List all topic
```sh
/usr/local/kafka/bin/kafka-topics.sh --list --bootstrap-server localhost:9092

```

# Remove Topic
```sh
/usr/local/kafka/bin/kafka-topics.sh --delete --topic <topic-name> --bootstrap-server localhost:9092

```


# Describe Topic
```sh
/usr/local/kafka/bin/kafka-topics.sh --describe --topic <topic-name> --bootstrap-server localhost:9092

```

# Information about Kafka brokers
```sh
bin/kafka-broker-api-versions.sh --bootstrap-server localhost:9092

```


# Produce Message
```sh
# Send message
/usr/local/kafka/bin/kafka-console-producer.sh --topic <topic-name> --bootstrap-server localhost:9092

```

# Consume Message
```sh
# Receive message
/usr/local/kafka/bin/kafka-console-consumer.sh --topic <topic-name> --bootstrap-server localhost:9092 --from-beginning

```

# Information Broker
```sh
/usr/local/kafka/bin/kafka-topics.sh --describe --topic <topic-name> --bootstrap-server localhost:9092

```

# Status of Cluster
```sh
/usr/local/kafka/bin/kafka-topics.sh --zookeeper localhost:2181 --describe

```
