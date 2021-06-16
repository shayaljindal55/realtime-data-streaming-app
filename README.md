Useful Commands :
&nbsp;
Trigger producer : node ./producer.js
&nbsp;
Trigger consumer : node ./consumer.js
&nbsp;
Start Kafka on Local (Windows 10) : bin/windows/kafka-server-start.bat ./config/server.properties
&nbsp;
Start Zookeeperfka on Local (Windows 10) : bin/windows/zookeeper-server-start.bat ./config/zookeeper.properties
&nbsp;
List all Kafka topics on Local (Windows 10) : ./bin/windows/Kafka-topics.bat --list --zookeeper localhost:2181
&nbsp;
Create a topic using command line: ./kafka-topics.sh --create --zookeeper <ZOOKEEPER_URL:PORT> --replication-factor <NO_OF_REPLICATIONS> --partitions <NO_OF_PARTITIONS> --topic <TOPIC_NAME>
&nbsp;
&nbsp;
&nbsp;

In case of the below error:
&nbsp;
"Classpath is empty. Please build the project first."
&nbsp;
&nbsp;

Follow the below solution:
&nbsp;
Change "log.dirs" in the config/server.properties file from "/tmp/kafka-logs" to "<COMPLETE PATH TO YOUR KAFKA-LOGS DIRECTORY>
&nbsp;
If "kafka-logs" directory does not exist, create one under your extracted kafka directory.
&nbsp;
Download KAFKA binaries from "https://www.apache.org/dyn/closer.cgi?path=/kafka/2.3.0/kafka_2.12-2.3.0.tgz" and extract the archive
&nbsp;