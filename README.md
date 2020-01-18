# kafka
run kafka before run project
 - bin/zookeeper-server-start.sh config/zookeeper.properties
 - bin/kafka-server-start.sh config/server.properties
 - bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic test
 - bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning


Message receive in terminal run:  bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning
