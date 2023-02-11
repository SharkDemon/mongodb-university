# MongoDB CRUD Operations: Insert and Find Documents

## Lesson 1: Inserting documents in a MongoDB collection

What methods are available in MongoDB for inserting a single document? (Select one.)

* .insertOne() (*)
* .inserting()
* .InsertDocument()
* .insertMany()

***

What methods are available in MongoDB for inserting multiple documents? (Select one.)

* .InsertDocument()
* .inserting()
* .insertOne()
* .insertMany() (*)

## Lesson 2: Finding documents in a MongoDB collection

What methods are available in MongoDB for finding documents? (Select one.)

* .find() (*)
* .query()
* .finding()
* .search()

***

The ```$in``` operator allows you to select all documents that have a field value equal to any of the values that are specified in the array.

* True (*)
* False

## Lesson 3: Finding documents by using comparison operators

Which of the following are comparison operators in MongoDB? Select all that apply.

* $gte (*)
* $lte (*)
* $eql
* $lt (*)
* $gt (*)

***

To use a comparison operator, we specify a field followed by the comparison operator and a value.

* True (*)
* False

## Lesson 4: Querying on array elements in MongoDB

Which of the following operators can be used to find a subdocument that matches specific criteria in an array?

* &element
* $elemMatch (*)
* $subMatch
* $docMatch

***

The following query will return only documents where the ```genre``` field is equal to a scalar value of ```Historical```:

```
db.books.find({ genre: "Historical" })
```

* True
* False (*)

## Lesson 5: Finding documents by using logical operators

Which of the following are logical operators in MongoDB? Select all that apply.

* &why
* $and (*)
* $or (*)
* $&&

***

Logical operators cannot be used in conjunction with each other.

* True
* False (*)
