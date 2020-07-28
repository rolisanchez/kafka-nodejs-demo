# Instructions

(In the folder that contains Kafka binaries and config)
First run Zookeper:
bin/zookeeper-server-start.sh config/zookeeper.properties

Then start the Kafka Server:
bin/Kafka-server-start.sh config/server.properties

To create a new topic manually from terminal:

../../kafka_2.12-2.3.0/bin/kafka-topics.sh --create --zookeper <ZOOKEEPER_URL:PORT> --replication-factor <NO_OF_REPLICATIONS> --partitions <NO_OF_PARTITIONS> --topic <TOPIC_NAME>

Consume using Kafka consumer:
bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic kafka-example-topic  --from-beginning

(In our project's folder)
To run producer:
./start.sh 

Run consumer:
node ./consumer.js