Hi,

To run this you need

A Storm cluster 
Kafka
A visualisation tool : Tableau or Spotfire

Recommended is Hortonworks Sandbox 2.1

Download and run the sandbox

It already has all the setup

Configure and check

Storm Nimbus server 
Storm Zookeeper
Strom Supervisor 
Storm UI

Run the code in tutorial 1 by deploying a jar  
Compile the project with maven

Run the Kafka file
java -cp target/Tutorial-1.0-SNAPSHOT.jar com.hortonworks.tutorials.tutorial1.TruckEventsProducer 
localhost:9092 localhost:2181 &

Deploy the storm file
storm jar target/Tutorial-1.0-SNAPSHOT.jar com.fusion.tutorials.tutorial2.TruckEventProcessingTopology

You will see the strom topology submitted and spots and bolts getting events

Persisting data in hdfs and hbase
The code for this is in tutorial 3

It will be seen on the Storm UI  a s we a re running the jar already 

Check for data in HBase shell and 

Hdfs  http://localhost:8000/filebrowser/view/truck-events-v4/staging


Visualisation

Install Tibco Spotfire and hortonworks ODBC drivers

Set them up for connecting to a hiveserver

Visualize the data real time!!!!




