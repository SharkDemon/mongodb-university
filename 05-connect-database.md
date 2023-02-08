# Connecting to a MongoDB Database

## Lesson 1: Using MongoDB connection strings

Which of the pre-formatted connection strings are available in the Atlas dashboard? (Select all that apply.)

* Connect with the MongoDB Shell (*)
* Connect your application (*)
* Connect using MongoDB Compass (*)
* Connect with MongoDB Charts

***

Click each option, followed by its corresponding match below.

* mongodb+srv:// (mongodb://)
* MDBUser:university01@ (username:password@)
* @mdb-training-cluster.swn5.mongodb.net (host[:port])
* ?retryWrites=true&w=majority (?\<options\>)

## Lesson 2: Connecting to a MongoDB Atlas cluster with the shell

Which REPL environment does the MongoDB Shell use? (Select one.)

* Pyton
* Node (*)
* Bash
* Perl

***

After you've installed mongosh, run ```mongosh -help``` in your terminal. Select all of the options that appear in the terminal from the following list: (Select all that apply.)

* --help (*)
* --container
* --host (*)
* --file (*)

## Lesson 3: Connecting to a MongoDB Atlas cluster with Compass

Open MongoDB Compass on your computer. From the following list, select all of the tabs that appear in the Compass UI: (Select all that apply.)

* Clusters
* My Queries (*)
* Performance (*)
* Databases (*)

***

Which of the following describes MongoDB Compass? (Select one.)

* A Node.js REPL environment that is used to interact with the database
* A data visualization tool that allows you to create and embed visualizations in your application
* A tool that allows you to query, transform, and move data across Amazon S3 and Atlas clusters
* A graphical user interface (GUI) for querying, aggregating, and analyzing data in MongoDB (*)

## Lesson 4: Connecting to a MongoDB Atlas cluster from an application

What does a MongoDB driver do? (Select one.)

* Executes an aggregation pipeline
* Connects MongoDB to applications via programming languages (*)
* Controls replication and sharding across servers
* Creates different types of charts of our data

***

Visit the official MongoDB driver documentation. Which of the following languages have drivers that are supported by MongoDB? (Select all that apply.)

* C# (*)
* Go (*)
* Node (*)
* Pascal

## Lesson 5: Troubleshooting MongoDB Atlas connection errors

How can you fix the following error? (Select one.)

```
MongoServerSelectionError: connection <monitor> to 34.239.188.169:27017 closed
```

* Update database access with the correct user credentials.
* Add your IP address in the Network Access panel in Atlas. (*)
* Create a new database on your Atlas cluster.

***

How can we fix the following error? (Select all that apply.)

```
MongoServerError: bad auth : Authentication failed.
```

* Check that you are connecting to the correct database deployment. (*)
* Update your IP address in the Network Access panel.
* Check that your username and password are spelled correctly in your connection string. (*)
