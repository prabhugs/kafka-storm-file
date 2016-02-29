# kafka-storm-file
Example basic storm topology to consume Kafka topics and write them to a file

### Build locally
    $ mvn clean package
This generates the kafka-storm-file-0.0.1-SNAPSHOT.jar file.

### Run
    $ cd /path/to/storm
    $ ./bin/storm jar /path/to/repo/target/kafka-storm-file-0.0.1-SNAPSHOT.jar com.storm.KafkaStormTopology

### Result
The Kafka topic('first-topic' in this case) is consumed and the messages are written in /tmp/stormoutput.txt file
