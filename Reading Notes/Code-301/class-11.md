# Class 11

## [nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

### Fill in the chart below with five differences between SQL and NoSQL databases

### What kind of data is a good fit for an SQL database?

    Data that would be stored in tables

### Give a real world example

    CREATE TABLE  "AGENTS" 
      (
        "AGENT_CODE" CHAR(6) NOT NULL PRIMARY KEY, 
      "AGENT_NAME" CHAR(40), 
      "WORKING_AREA" CHAR(35), 
      "COMMISSION" NUMBER(10,2), 
      "PHONE_NO" CHAR(15), 
      "COUNTRY" VARCHAR2(25)  );

### What kind of data is a good fit a NoSQL database?

    A collection of Key value pairs

### Give an real world example

    {
        name: "John",
          age : 35,
          dob : ISODate("01-05-1990"),
          profile_pic : "https://example.com/john.jpg",
          social : {
                twitter : "@mongojohn",
                    linkedin : "https://linkedin.com/abcd_mongojohn"
                  }
    }

### Which type of database is best for hierarchical data storage?

    NoSQL Databases

### Which type of database is best for scalability?

    SQL Databases

## Bookmark/Skim

[mongoose api](https://mongoosejs.com/docs/api.html#Model)

[React Router](https://reactrouter.com/web/api/BrowserRouter)

## Videos

## [sql vs nosql (Video)](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

### What does SQL stand for?

    Structured Queried Language

### What is a relational database?

    A relational database is a type of database that focuses on the relation between stored data elements.

### What type of structure does a relational database work with?

    Tables with collumns and rows 

### What is a ‘schema’?

    A data structure 

### What is a NoSQL database?

    A large database with no schema 

### How does it work?

    All of the data is placed in one place and accessed when needed

### What is inside of a Mongo database?

    One or more collections of documents. Example of collection:
    {
    "name": "Everest",
    "height": 8848,
    "location": ["Nepal", "China"],
    "ascents": {
        "first": {
            "year": 1953,
        },
        "first_winter": {
            "year": 1980,
        },
        "total": 5656,
    }
}

### Which is more flexible - SQL or MongoDB? and why

    The schemaless design of MongoDB documents makes it easy to build and enhance applications over time

### What is the disadvantage of a NoSQL database?

    MongoDB uses a lot of memory for data storage.
    There is a limit to the document size, which is 16 MB.
    There is no transaction support in MongoDB
