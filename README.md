

## Druid : 
 Druid is a high performance, real-time analytics database that delivers sub-second queries on streaming and batch data at scale and under load.
    
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
