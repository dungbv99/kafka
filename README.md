# kafka with java

Learn to use kafka to send and receive message

<H1>Run project</H1>

<h2>Start kafka and zookeeper</h2>
- bin/zookeeper-server-start.sh config/zookeeper.properties
 - bin/kafka-server-start.sh config/server.properties
 - bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic test
 - bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning

<h2>Run java code </h2>
- mvn clean package
- java -jar target/serving-web-content-0.0.1-SNAPSHOT.jar


Message receive in terminal run:  bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning
