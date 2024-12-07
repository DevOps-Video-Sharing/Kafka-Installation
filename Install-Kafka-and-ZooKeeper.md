```sh
#Download
wget https://downloads.apache.org/kafka/3.6.0/kafka_2.12-3.8.0.tgz
```

```sh
#unzip
sudo tar -xvf kafka_2.12-3.8.0.tgz -C /usr/local
```

```sh
#move
sudo mv /usr/local/kafka_2.12-3.8.0 /usr/local/kafka
```


```sh
#start zookeeper
cd /usr/local/kafka
bin/zookeeper-server-start.sh config/zookeeper.properties
```

```sh
#start kafka
cd /usr/local/kafka
bin/kafka-server-start.sh config/server.properties
```


```sh
#error to start zoopkeeper
sudo mkdir /usr/local/kafka/logs
sudo chown dat:dat /usr/local/kafka/logs
#start again
cd /usr/local/kafka
bin/zookeeper-server-start.sh config/zookeeper.properties
```
