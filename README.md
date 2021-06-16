Useful Commands :
Trigger producer : node ./producer.js
Trigger consumer : node ./consumer.js
Start Kafka on Local (Windows 10) : bin/windows/kafka-server-start.bat ./config/server.properties
Start Zookeeperfka on Local (Windows 10) : bin/windows/zookeeper-server-start.bat ./config/zookeeper.properties
List all Kafka topics on Local (Windows 10) : ./bin/windows/Kafka-topics.bat --list --zookeeper localhost:2181
Create a topic using command line: ./kafka-topics.sh --create --zookeeper <ZOOKEEPER_URL:PORT> --replication-factor <NO_OF_REPLICATIONS> --partitions <NO_OF_PARTITIONS> --topic <TOPIC_NAME>

In case of the below error:
"Classpath is empty. Please build the project first."

Follow the below solution:
Change "log.dirs" in the config/server.properties file from "/tmp/kafka-logs" to "<COMPLETE PATH TO YOUR KAFKA-LOGS DIRECTORY>
If "kafka-logs" directory does not exist, create one under your extracted kafka directory.

Download KAFKA binaries from "https://www.apache.org/dyn/closer.cgi?path=/kafka/2.3.0/kafka_2.12-2.3.0.tgz" and extract the archive
