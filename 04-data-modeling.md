# Introduction to MongoDB Data Modeling

## Lesson 1: Introduction to data modeling

Which of the following statements is/are true about data modeling? (Select all that apply.)

* Data modeling is the process of defining how data is stored. (*)
* Data modeling is the process of defining the relationships that exist among different entities in your data. (*)
* Data modeling is the process of collecting data.

***

Which of the following are benefits of a proper data model? (Select all that apply.)

* A proper data model makes it easier to manage your data. (*)
* A proper data model makes queries more efficient. (*)
* A proper data model uses less memory and CPU. (*)
* A proper data model reduces costs. (*)

***

Which of the following is a benefit of the document model?

* The document model does not enforce any document structure by default. This means that documents even in the same collection can have different structures. (*)
* The document model makes having a schema useless.
* The document model supports only simple relationships among data to make data wrangling easier.

## Lesson 2: Types of data relationships

Which of the following are common types of relationships that are found in every database? (Select all that apply.)

* One-to-one relationship (*)
* One-to-many relationship (*)
* Many-to-many relationship (*)
* One-to-zillions relationship

***

What is the type of relationship shown in the following document?

```
{
    "_id": ObjectId("00000001"),
    "name": "Marnie Dupree",
    "grade": "Freshman",
    "studentId": 123456,
    "email": "mdupree@college.edu"
}
```

* One-to-one relationship (*)
* One-to-many relationship
* Many-to-many relationship

## Lesson 3: Modeling data relationships

A legacy bank database has been ported to MongoDB, resulting in a set of collections that were mapped to their original tables.

You're tasked with redesigning the accounts collection of the banking database to make the information clearer. The bank would like you to keep the customers' contact information and account information separate.

The following is a sample document in the accounts collection:

```
{
  "account_id": "MDB653115886",
  "account_holder": "Herminia Mckinney",
  "account_type": "savings",
  "balance": 6617.34,
  "street_num": 123,
  "street": "Main St",
  "city": "Tulsa",
  "state": "OK",
  "zip": 74008,
  "country": "USA",
  "home_phone": 1234567890,
  "cell_phone": 1111111111,
  "transfers": [
    ...
  ],    
}
```

Which of the following actions can be made to improve this schema? Consider the following requirements:

* Preserve the one-to-one relationship among all the fields.
* Keep the contact and account information separate.
* Store data together that is accessed together.

Hint

Remember that you can embed subdocuments and create separate collections.

* Create two collections: one for accounts and one for customer_info. (*)
*  Embed the phone numbers as a subdocument. (*)
* Create two collections that have no overlapping fields.
* Keep the current schema as is.

***

Consider a banking database that stores information on customers, such as their contact information, account information, and all account activity information. A one-to-many relationship exists between the customer and their transactions.

Which of the following are valid ways to represent this one-to-many relationship between the customer and their transactions? (Select all that apply.)

* Create two collections: one collection for the customers' identifying information and one collection for the transactions. In the transactions collection, each document contains a customer's transactions and a field to reference the customer's information document. (*)
* Create a collection that contains documents for each customer. The document contains embedded subdocuments for the contact information and account information, as well as an array that holds all their transactions.
* Embed the transactions for each customer as an array of subdocuments in the corresponding customer document. (*)

## Lesson 4: Embedding data in documents

Which of the following statements is/are true about embedding data in documents? (Select all that apply.)

* Embedding data in documents simplifies queries. (*)
* Embedding data in documents improves the overall performance of queries. (*)
* Embedding data in documents makes your document smaller over time.
* Embedding data in documents never results in an unbounded document.

***

Which of the following relationship types often use embedding? (Select all that apply.)

* One-to-one relationship
* One-to-many relationship (*)
* Many-to-many relationship (*)

## Lesson 5: Referencing data in documents

Which of the following statements is/are true about referencing data in documents? (Select all that apply.)

* Referencing data in documents avoids duplication of data. (*)
* Referencing data in documents may result in smaller documents. (*)
* Referencing data in documents links documents by using the same field. (*)
* Referencing data in documents improves read performance.

***

Consider the following document, which contains data about a blog post and its comments. Which field is used as a reference?

```
{
    "author": "Aileen Long",
    "title": "Learn MongoDB in 30 Mins",
    "published_date": ISODate("2020-05-18T14:10:30Z"),
    "tags": ["mongodb", "introductory", "database", "nosql"],
    "comments":
        {
            "comment_id": "LM001",
            "reader_id": "AL001",
            "comment_date": ISODate("2020-05-19T14:22:00Z"),
            "comment": "Great read!"
        },
        {
            "comment_id": "LM002",
            "reader_id": "AL002",
            "comment_date": ISODate("2020-06-01T08:00:00Z"),
            "comment": "So easy to understand - thanks!"
        }
}
```

* comment_id (*)
* comments
* date
* reader_id

## Lesson 6: Scaling a data model

What are the effects of creating unbounded documents when embedding data? (Select all that apply.)

* Unbounded documents impact write performance. (*)
* Unbounded documents improve pagination performance.
* Unbounded documents cause storage problems. (*)

***

What is the recommended way to avoid the unbounded document sizes that may result from embedding?

* Break data into multiple collections and use references. (*)
* Break data into multiple databases.
* Separate documents to store on different servers.

***

What is MongoDB's principle for how you should design your data model?

* Data that is accessed together should be stored together. (*)
* Data that is collected in the same day should be stored together.
* Data that is not in a one-to-one relationship should be stored together.

## Lesson 7: Using Atlas tools for schema help

Which tab in Data Explorer shows ways to improve your schemas?

* Indexes
* Schema Anti-Patterns (*)
* Find

***

What is the minimum Atlas Cluster tier that you must have to use the Performance Advisor tool?

* M0
* M10 (*)
* M30

