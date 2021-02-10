# streaming_data_pipeline

Tech Stack: hadoop Distributed File System, Spark, Apache Kafka, Spark Streaming, Python, PostgreSQL, Django, Flexmonster 

The data streaming is generated for every 1 second, events in the form of JSON string message are stored in the topic in Kafka.

Events are consumed from the topic using Streaming Data Pipeline(Spark Structured Streaming). Consumed data is transformed, processed and aggregated data is stored in the 
PostgreSQL database table and raw data is stored in the persistent storage at specified micro batch interval. 

Raw data is stored in persistent storage(Hadoop Distribited File System) 

Aggregated data is stored in the PostreSQL database table.

Aggregated data is visualized in the form of Chart and Data Table(Django, Flexmonster)
