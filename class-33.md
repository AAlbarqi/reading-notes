# Data Modeling & NoSQL Databases

#### SQL vs NoSQL

![](https://cryptoinvestinginsider.com/blog/wp-content/uploads/2019/07/12AZ5SpsmDvk67BIImwHvh_cQ.png)

- SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.
- SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. 
- SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.
- SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable.
- SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb

#### NOSQL DATA MODELING TECHNIQUES

- NoSQL data modeling often starts from the application-specific queries as opposed to relational modeling:
    - Relational modeling is typically driven by the structure of available data. The main design theme is  “What answers do I have?” 
    - NoSQL data modeling is typically driven by application-specific access patterns, i.e. the types of queries to be supported. The main design theme is “What questions do I have?”  

- Conceptual Techniques:
1. Denormalization
2. Aggregates
3. Application Side Joins

- General Modeling Techniques
1. Atomic Aggregates
2. Enumerable Keys
3. Dimensionality Reduction
4. Index Table
5. Composite Key Index
6. Aggregation with Composite Keys
7. Inverted Search – Direct Aggregation

#### Discussion

- 3 advantages to Test Driven Development:
    1. You receive fast feedback.
    2. TDD creates a detailed specification.
    3. TDD reduces time spent on rework.

- In what case would you need to use beforeEach() or afterEach() in a test suite?
    - If you have some work you need to do repeatedly for many tests

- What is one downside of Test Driven Development?
    1. It necessitates a lot of time and effort up front, which can make development feel slow to begin with.
    2. Focusing on the simplest design now and not thinking ahead can mean major refactoring requirements.
    3. It's difficult to write good tests that cover the essentials and avoid the superfluous.

- What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
    - The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.

- Name a use case for a static method.
    - Use static when you want to provide class level access to a method.

#### Terms

- functional programming : is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects.

- pure function : is a function where the return value is only determined by its input values, without observable side effects.

- higher-order function :  is a function that can take another function as an argument, or that returns a function as a result.

- immutable state : cannot be modified after it is created.

- object : containers for named values, called properties and methods. 

- object-oriented programming (OOP) :  is a programming paradigm based on the concept of "objects", which can contain data and code: data in the form of fields, and code, in the form of procedures. 

- class : is a type of function, but instead of using the keyword function to initiate it, we use the keyword class , and the properties are assigned inside a constructor()

- prototype : The prototype is an object that is associated with every functions and objects by default in JavaScript, where function's prototype property is accessible and modifiable and object's prototype property (aka attribute) is not visible.

- super : The super keyword is used to access and call functions on an object's parent.

- inheritance : is the mechanism of basing an object or class upon another object (prototype-based inheritance) or class (class-based inheritance), retaining similar implementation.

- constructor : is a block of code that initializes the newly created object.

- instance : is an object containing data and behavior described by the class. 

- context : It refers to the object within the function being executed.

- this : refers to the object that the function is executing in. this is determined by how a function is invoked.

- Test Driven Development (TDD) : is a software development process that relies on the repetition of a very short development cycle: requirements are turned into very specific test cases, then the code is improved so that the tests pass.

- Jest :  is a JavaScript testing framework maintained by Facebook, Inc. with a focus on simplicity.

- Continuous Integration (CI) : is the practice of merging all developers' working copies to a shared mainline several times a day.

- unit test : is a level of software testing where individual units/ components of a software are tested. 
