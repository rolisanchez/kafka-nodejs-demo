## Instructions
To create a new topic manually from terminal:

../../kafka_2.12-2.3.0/bin/kafka-topics.sh --create --zookeper <ZOOKEEPER_URL:PORT> --replication-factor <NO_OF_REPLICATIONS> --partitions <NO_OF_PARTITIONS> --topic <TOPIC_NAME>

Or run createTopic.js