# Connecting to MongoDB in Java

## Lesson 1: Using MongoDB Java client libraries

What is the principal responsibility of a MongoDB driver? (Select one.)

* To execute an aggregation pipeline.
* To establish secure connections to a MongoDB cluster and execute database operations on behalf of client applications. (*)
* To control replication and sharding across servers.
* To create different types of charts of our data.

***

The official MongoDB drivers adhere to each programming language’s best practices.

* True (*)
* False

## Lesson 2: Connecting to an Atlas cluster in Java applications

How do you connect your Java application to your Atlas cluster? (Select one.)

* Create a MongoClient object from a connection string. (*)
* Pass the connection string into a MongoClient object.
* Create a new cluster with the same name as your application.

***

According to the documentation, what are two build systems that can be used to add the MongoDB Java driver as a dependency in your Java application? (Select all that apply.)

* Maven (*)
* Jenkins
* Gradle (*)
* Ant

***

How many MongoClient instances should your application have for a single Atlas cluster? (Select one.)

* 0
* 1 (*)
* 2
* 3 or more

## Lesson 3: Troubleshooting a MongoDB connection in Java applications

What are the potential causes of the following error in a Java application? (Select all that apply.)

```
Command failed with error 8000 (AtlasError): 'bad auth : Authentication failed.' on server cluster0-shard-00-02.zuxlr.mongodb.net:27017. The full response is {"ok": 0, "errmsg": "bad auth : Authentication failed.", "code": 8000, "codeName": "AtlasError"}
```

* The database user is missing (*)
* The IP address that the user is connecting from is incorrect
* The username and/or password in the connection string is incorrect or misspelled (*)

***

What can cause the following error in a Java application? (Select one.)

```
An exception occured while executing the Java class. Timed out after 30000 ms while waiting for a server that matches com.mongodb.client.internal.MongoClientDelegate$1@41599ac0. Client view of cluster state is {type=REPLICA_SET, servers=[{address=cluster0-shard-00-00.zuxlr.mongodb.net:27017, type=UNKNOWN, state=CONNECTING, exception={com.mongodb.MongoSocketReadException: Prematurely reached end of stream}}, {address=cluster0-shard-00-01.zuxlr.mongodb.net:27017, type=UNKNOWN, state=CONNECTING, exception={com.mongodb.MongoSocketReadException: Prematurely reached end of stream}}, {address=cluster0-shard-00-02.zuxlr.mongodb.net:27017, type=UNKNOWN, state=CONNECTING, exception={com.mongodb.MongoSocketReadException: Prematurely reached end of stream}}]
```

*  The user's current IP address is not on their IP access list in Atlas. (*)
* The user entered incorrect database user credentials.
* The user attempted to access a terminated Atlas cluster.
* The user attempted to write to a database but has read-only privileges.
