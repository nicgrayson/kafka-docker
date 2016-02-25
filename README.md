# kafka-docker
Builds docker image to run kafka scripts

# Install
`docker pull nicgrayson/kafka`

# List included scripts
`docker run -it --rm nicgrayson/kafka`

# Examples

## Describe all topics
`docker run -it --rm nicgrayson/kafka ./kafka-topics.sh --zookeeper zookeeper:2181/kafka --describe`

## Run a simple shell consumer
`docker run -it --rm kafka ./kafka-simple-consumer-shell.sh --broker-list broker-0:9092 --topic est --partition 0`
