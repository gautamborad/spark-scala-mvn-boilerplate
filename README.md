# Spark + Scala Boilerplate Project


## Prerequisites

Download and install the latest version of Spark on your system with these commands.

```
wget https://d3kbcqa49mib13.cloudfront.net/spark-2.1.1-bin-hadoop2.7.tgz
tar -xvzf spark-2.1.1-bin-hadoop2.7.tgz
sudo mv spark-2.1.1-bin-hadoop2.7 /usr/local/spark
echo 'export PATH=$PATH:/usr/local/spark/bin' >> ~/.bashrc
source ~/.bashrc
```

You can verify the installation by the following command, which should launch spark shell.

```spark-shell```


### Building the project
```
mvn package
```

### Running the project
The command for running the jar file created by build phase is:

```spark-submit --class com.examples.MainExample --master local[2] target/spark-scala-maven-project-0.0.1-SNAPSHOT-jar-with-dependencies.jar```



