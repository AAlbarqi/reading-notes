# Advanced Mongo/Mongoose

#### Repository-design-pattern

- a design pattern is a reusable solution to a general problem occurring in a given context in software design. A design pattern is not a design which is directly transferred into code(source or machine).

- Repository pattern separates the data access logic and maps it to the business entities in the business logic.
![](https://cubettech.com/wp-content/uploads/2015/07/Reposiory-Design-Pattern.png)

To put it simply, Repository pattern is a kind of container where data access logic is stored. It hides the details of data access logic from business logic. In other words, we allow business logic to access the data object without having knowledge of underlying data access architecture.

#### mongodb-memory-server

- Simply put, it allows us to start a mongod process that stores the data in memory. 

**Pros:**

1. No need for mocks.
2. Faster development.
3. More reliable tests.
4. Tests are easier to build.

**Cons:**

1. The in-memory database probably needs seeding
2. More memory usage (dah)
3. Tests take longer to run (depending on your hardware).

# Discussion

- Why would a developer choose to make data models?
    - A data model helps design the database at the conceptual, physical and logical levels. Data Model structure helps to define the relational tables, primary and foreign keys and stored procedures. 

- What purpose do CRUD operations serve?
    - create, read (aka retrieve), update, and delete (CRUD) are the four basic functions of persistent storage.

- What kind of database is Postgres? What kind of database is MongoDB?
    - PostgreSQL is a traditional RDBMS (relational database management system) SQL database.
    - MongoDB is a cross-platform document-oriented database program. Classified as a NoSQL database program.

- What is Mongoose and why do we need it?
    - Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node. ... It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.

- Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.
     - A reservation system, Users, places, and dates. Each user reserves different places on different dates, each place is booked by different users on different dates.

# Terms

- database : an organized collection of data, generally stored and accessed electronically from a computer system. 

- data model : an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities.

- CRUD : create, read (aka retrieve), update, and delete (CRUD) are the four basic functions of persistent storage.

- schema : the organization of data as a blueprint of how the database is constructed.

- sanitize : Clean up user-submitted HTML, preserving whitelisted elements and whitelisted attributes on a per-element basis.

- Structured Query Language (SQL): a domain-specific language used in programming and designed for managing data held in a relational database management system, or for stream processing in a relational data stream management system. 

- Non SQL (NoSQL) : a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases.

- MongoDB : a cross-platform document-oriented database program.

- Mongoose : an Object Data Modeling (ODM) library for MongoDB and Node. js.

- record : A record is composed of fields and contains all the data about one particular person, company, or item in a database.

- document : a type of nonrelational database that is designed to store and query data as JSON-like documents. 

- Object Relation Mapping (ORM) : a programming technique for converting data between incompatible type systems using object-oriented programming languages. 