## Room :
  * Room is an ORM, Object Relational Mapping library. In other words, Room will map our database objects to Java objects.
* The benefits  by the room
- 1 - Check compile time for SQL queries.  
 - 2 - Convenient annotations that reduce redundant and error-prone standard code.
 - 3 - Simplified database migration paths.  
* three major components in Room :
- 1 - database class .  
 - 2 - Data entities .
 - 3 - Data access objects (DAOs) . 
 * this three components are  holding the database ,provide methods that your app can use to query, update, insert, and delete data in the database and  provides your app with instances of the DAOs associated with that database
  
  ### Defining data using Room entities :
   you can use Room entities to define your database schema without writing any SQL code.
   
   * primary key : Each Room entity must define a primary key that uniquely identifies each row in the corresponding database table.
   
