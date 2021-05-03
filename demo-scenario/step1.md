This is your first step.

## Task

Change directory to Kafka home:

`cd kafka`{{execute}}

Create topic:

`./bin/kafka-topics.sh --create --topic quickstart-events --bootstrap-server localhost:9092`{{execute}}

Describe topic: 

`./bin/kafka-topics.sh --describe --topic quickstart-events --bootstrap-server localhost:9092`{{execute}}

Produce event (reading from stdin):

`./bin/kafka-console-producer.sh --topic quickstart-events --broker-list localhost:9092`{{execute}}

Consume events (to stdout):

`./bin/kafka-console-consumer.sh --topic quickstart-events --from-beginning --bootstrap-server localhost:9092`{{execute}}
