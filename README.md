# kafkaClusteDockerCompose

Docker compose project to have a Kafka Cluster with a Zookeeper Cluster.

## Running

After clone this repository in local, run:

```bash
~$ docker-compose up
```

This project uses [Wurstmeister/Kafka](https://github.com/wurstmeister/kafka-docker) docker image, visit its README to get more info.

## Testing

Install in your environment [kafkacat](https://github.com/edenhill/kafkacat), to be able to test your cluster (consume, produce, get info and so on).

After install it, for example, you can get info about the cluster as given below:

```bash
~$ kafkacat -L -b localhost
Metadata for all topics (from broker -1: localhost:9092/bootstrap):
 3 brokers:
  broker 2 at kafka3:9094
  broker 1 at kafka2:9093
  broker 0 at kafka1:9092
 0 topics:
```
