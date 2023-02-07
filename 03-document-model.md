# MongoDB and the Document Model

## Lesson 1: Introduction to MongoDB

What is the relationship between the MongoDB database and MongoDB Atlas? (Select one.)

* The MongoDB database is the locally deployed version of MongoDB Atlas.
*  The MongoDB database is a core element of MongoDB Atlas, which is a multi-cloud developer data platform. (*)
* The MongoDB database is the free version of MongoDB Atlas.

***

Jenni works at an e-commerce start-up that uses MongoDB for its customer data managament, product catalog and payment processing. Her startup now wants to add personalized recommendations for customers using real-time analytics. Jenni and her team will need to move data to a separate analytics database to handle this new use case.

* True.
* False. (*)

***

What is the basic unit of data in MongoDB? (Select one.)

* Collection
* Database
* Document (*)
* Row

## Lesson 2: The MongoDB document model

Which of the following are data types that are supported by MongoDB by using BSON? (Select all that apply.)

* 32-bit integer (*)
* Object (*)
* Array (*)
* ObjectId (*)
* _id
* All of the above.

***

Which of the following statements are true about the _id field in MongoDB? (Select all that apply.)

* The user must specify the _id field for each inserted document.
* The _id field is required for each document. (*)
* The _id field must be unique. (*)
* The _id field is automatically included and populated with an ObjectId if the _id field is omitted in an inserted document. (*)

***

Use the following documents labeled Document A and Document B to answer this question.

Elena's company has been storing customer data in records that are structured like Document A. Her company wants to add a new field to their customer records so that they are structured like Document B. Before inserting records like Document B, Elena and her team must update all older records to include the new field.

**Document A**
```
{
  "username": "vreddy",
  "name": "Vasanti Reddy",
  "email": "vreddy1@gmail.com",
  "location": {
    "city": "Delhi",
    "country": "India"
  }
}
```
**Document B**
```
{
  "username": "avasa",
  "name": "Asad Vasa",
  "email": "avasa1@yahoo.com",
  "social_media": {
    "Twitter": "avasa",
    "Instagram": "Asad101",
    "LinkedIn": "AsadVasa"
  },
  "location": {
    "city": "Los Angeles",
    "country": "United States"
  }
}
```
* True
* False (*)

## Lesson 3: Managing databases, collections, and documents in Atlas data explorer

Which of the following are databases in your MongoDB Atlas cluster? (Select all that apply.)

* sample_supplies (*)
* sample_analytics (*)
* sales
* sample_music

***

Which of the following are collections in the sample_analytics database? (Select all that apply.)

* accounts (*)
* companies
* customers (*)
* transactions (*)

***

What is the current Documents Size of the library database? (Select one.)

* 0B (*)
* 4KB
* 8KB

***

How many collections now exist in the library database? (Select one.)

* 0
* 1
* 2 (*)
