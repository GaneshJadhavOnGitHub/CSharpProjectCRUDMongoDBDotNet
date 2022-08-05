# CSharpProjectCRUDMongoDBDotNet
CRUD Functionality with MONGODB and Dot net framework.

** CRUDMONGODB
---------------------
Program Requirements
-------------------------------------------------------------------------------------------------------------------------------------------
Operating System  - Windows 10 Pro Version 21H1 (OS Build 19043.1645)

Dot Net Framework - 4.7.2

MongoDB Server Version - 5.0.3

MongoDB shell version - v5.0.3

MongoDB Compass Version - 1.28.4

-------------------------------------------------------------------------------------------------------------------------------------------

Required Libraries :- 
-------------------------------------------------------------------------------------------------------------------------------------------

Install Following packges using nuget.

1. MongoDB.Driver -: Official .NET driver for MongoDB.


2. MongoDB.Bson  -: MongoDB's Official Bson Library.


Go to Tools -> NuGet Package Manager -> Package Manager Console

Type following commands in Package Manager Console 

Install-Package MongoDB.Driver -Version 2.15.1

Reference URL :- https://www.nuget.org/packages/mongodb.driver

Install-Package MongoDB.Bson -Version 2.15.1

Reference URL :- https://www.nuget.org/packages/mongodb.bson


-------------------------------------------------------------------------------------------------------------------------------------------


Description :- 
------------------

CRUD Functionality with MONGODB and Dot net framework.

C - Create , R - Read , U - Update , D - Delete

-------------------------------------------------------------------------------------------------------------------------------------------
Using MongoDB Compass , Do following things :- 

Create Database 'BoxOffice' in MongoDB.

Create Collection 'Movies' in Database 'BoxOffice'.

Don't select Capped Collection while creating Collection it will not allow to edit data later,
which is required by us.

Fields in Collection 'Movies' are as below - 


MovieId -          Int32

Title -            String

Production House - String

YearOfRelease -    Int32

BudgetCrores -     Decimal128

CollectionCrores - Decimal128

Verdict -          String

Insert data (documents) in the Collection.

-------------------------------------------------------------------------------------------------------------------------------------------

Please note :- While running program, MongoDB server must be running. 

To run MongoDB ,

Go to bin folder where MongoDB server is installed and type following command


mongod --dbpath="Path to the directory where we are storing the databases"

-------------------------------------------------------------------------------------------------------------------------------------------

Glossary :- 
-------------

BSON          :- MongoDB stores documents (objects) in a format called BSON. 
                 BSON is a binary serialization of JSON-like documents. 
                 BSON stands for “Binary JSON”, 
                 but also contains extensions that allow representation of data types that are not part of JSON. 
                 For example, BSON has a Date data type and BinData type.

Serialization :- Serialization in C# is the process of bringing an object into a form that can be written on stream.
                 It's the process of converting the object into a form so that it can be stored on a file, database, or memory;        
                 or, it can be transferred across the network.

------------------------------------------------------------------------------------------------------------------------------------------------
[CRUDWithMongoDBOutput](https://user-images.githubusercontent.com/86361080/183069135-2c755fd6-de77-44cb-b4d3-73fbd5d0efbe.jpg)

