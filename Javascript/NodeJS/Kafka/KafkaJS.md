# KafkaJS
Kafka is a Publish/Subscribe messaging system. It allows **producers** to write **_records_** into Kafka topics that can be read by one or more **consumers**. These records that cannot be deleted or modify once they are sent to Kafka (this is known as “distributed commit log”).

## Topic
A Topic is **a category/feed name to which records are stored and published**. As said before, all Kafka records are organized into topics. Producer applications write data to topics and consumer applications read from topics.

![[kafka logic.png]]

## Producer and Consumers
**Producers** are those client applications that publish (write) events to Kafka, and **consumers** are those that subscribe to (read and process) these events. In Kafka, producers and consumers are fully decoupled and agnostic of each other, which is a key design element to achieve the high scalability that Kafka is known for. For example, producers never need to wait for consumers. Kafka provides various guarantees such as the ability to process events exactly-once.

**DEFAULT PORT: 9092**

#NODEJS 