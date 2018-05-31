# Spring-Boot-Kafka-Producer-Example
Spring Boot Kafka Producer Example

Download and run kafka and uncompress:
-  Start Zookeeper
      bin/zookeeper-server-start.sh config/zookeeper.properties
-  Start Kafka:
      bin/kafka-server-start.sh config/server.properties
-  Create topic: 
      bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example
-  Testing consumer:  
      bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic Kafka_Example --from-beginning
      
-  Go to browser send message:      http://localhost:8081/kafka/public/Name
      
