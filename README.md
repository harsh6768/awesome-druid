

## Druid : 
 Druid is a high performance, real-time analytics database that delivers sub-second queries on streaming and batch data at scale and under load.
 
 Druid is an open-source data store designed for high-performance analytics on large volumes of data. It is built to handle real-time streaming data and can efficiently store, query, and analyze large amounts of event data.

Druid is designed for use cases that require fast, interactive exploration of data. It enables businesses to gain insights from real-time data streams and make data-driven decisions. It is particularly well-suited for applications such as monitoring, user analytics, fraud detection, log analysis, and time series analysis.

Key features of Druid include:

Real-time ingestion: Druid can ingest and process data in real time, making it ideal for streaming data sources like IoT devices or event-driven systems.

Columnar storage: Druid uses a columnar storage format optimized for fast analytical queries. This allows for efficient compression, faster query performance, and selective filtering of data.

Distributed architecture: Druid can be deployed in a distributed cluster to handle large datasets and provide horizontal scalability. It can scale horizontally by adding more nodes to the cluster.

Interactive queries: Druid supports fast, interactive queries on large data sets. It provides low-latency querying capabilities, allowing users to explore and visualize data in real time.

Aggregation and filtering: Druid supports advanced filtering and aggregation capabilities to perform complex analytical operations on data. It can efficiently handle group-by queries, time-based aggregations, and filtering based on dimensions or metrics.

Flexibility and extensibility: Druid provides a pluggable architecture that allows integration with various data sources and third-party tools. It supports a wide range of data formats and can be extended with custom modules and plugins.

Overall, Druid is a powerful data store that enables real-time analytics and exploration of large-scale data sets. It offers fast query performance, scalability, and flexibility, making it a popular choice for organizations dealing with high-velocity, time-series data.
  
  
  
  
### Official Website Link : https://druid.apache.org/

 <img width="1438" alt="druid image" src="https://github.com/harsh6768/awesome-druid/blob/master/Upload/druid1.png">


## Setup Druid on Mac System : If you have multiple version of java in mac system

#### 1. Download Druid from https://druid.apache.org/downloads.html official website
#### 2. Unzip tar.gz file
#### 3. Download java 8 or java 11 which are only supported by the druid as of now 
#### 4. Once java is installed , then create symlink using below command 
 
     ln -s /Library/Java/JavaVirtualMachines/jdk-11.0.17.jdk/Contents /Library/Java/JavaVirtualMachines/jdk-11.0.17.jdk

#### 5. Go to the /Library/Java/JavaVirtualMachines and run ls command to check which version of java is present 
#### 6. Open .bash_profile using text editor and add DRUID_JAVA_HOME path for java 8 or java 11 version
      
Command to edit .bash_profile 
     
    vi ~/.bash_profile
      
    
.bash_profile file

      
      JAVA_HOME="/Users/harsh/Downloads/jdk-17.0.2.jdk/Contents/Home"
      export JAVA_HOME

      M2_HOME="/Users/harsh/Downloads/apache-maven-3.8.5"
      export MAVEN_HOME

      // specific to druid only 
      DRUID_JAVA_HOME="/Users/harsh/Downloads/jdk-11.0.17.jdk/Contents/Home"
      export DRUID_JAVA_HOME

      PATH=$PATH:$JAVA_HOME/bin:$M2_HOME/bin
      export PATH


<img width="1438" alt=".bash_profile" src="https://github.com/harsh6768/awesome-druid/blob/master/Upload/Screenshot%202023-06-08%20at%2012.38.04%20PM.png">

#### Now go to the druid bin folder and run start-druid file with below command and make zookeeper is not running in local ,else it won't restart.

     ./start-druid
     
     
 
<img width="1438" alt="run druid server" src="https://github.com/harsh6768/awesome-druid/blob/master/Upload/Screenshot%202023-06-08%20at%2012.42.04%20PM.png">  
