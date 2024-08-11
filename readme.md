apt-get install build-essential librdkafka-dev -y

criar tópico
kafka-topics --create --topic=teste --bootstrap-server=localhost:9092 --partitions=3

monitorar consumer
kafka-console-consumer --bootstrap-server=localhost:9092 --topic=teste

monitorar group
kafka-consumer-groups --bootstrap-server localhost:9092 --describe --group=goapp-group2
