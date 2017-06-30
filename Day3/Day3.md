# Streaming workshop:

Task were distributed around the group. There is no cooperation or learning from each other at all.
My task: get the generator up and running.

* Step 1: 
Java projects received. 

* Step 2: 
Need to compile the java program. In order to do that, I installed IntelliJ on my Mac. 
I needed to add an additional idk on my Mac, because the cluster is running a idk 1.7

In IntelliJ, I needed to figure out how to compile the .java source and project into a .jar file. Google was helpful here.

Project compiled and transferred to 1 host in the cluster.

The generator starts with the following command:

/usr/java/jdk1.7.0_67-cloudera/bin/java -cp bootcamp-0.0.1-SNAPSHOT.jar com.cloudera.fce.bootcamp.MeasurementGenerator ip-172-31-47-120.us-west-2.compute.internal 9092

---

We are afraid that the generator generates too much data. So I added an additional feature into the data generator. With a 3rd parameter, you can now specify the number of milliseconds to wait before a new record is generated.

The new call is: 

/usr/java/jdk1.7.0_67-cloudera/bin/java -cp bootcamp-0.0.1-SNAPSHOT.jar com.cloudera.fce.bootcamp.MeasurementGenerator ip-172-31-47-120.us-west-2.compute.internal 9092 5000

This will wait 5 seconds before a new record is generated.

---

The rest of the day looked up the manual and looked at others. There is little to none cooperation in this group. Bad luck.

Back home, I'll run through the simple flume tutorial in order to get started.

Started on my own vm, using the cloudera manual tutorial.

https://www.cloudera.com/documentation/other/tutorial/CDH5/topics/ht_flume_to_hdfs.html


