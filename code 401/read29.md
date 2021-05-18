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
 * Using Room library, you can define entities that is related to what you want to store.

 - Room entities can be used to define database schema without writing any SQL code.

Each Room entity must be declared as a class that is annotated with @Entity, to includes the fields for each column in the entity.

Room uses the class name as the database table name, but it can be changed if you set the tableName property of the @Entity annotation an @ColumnInfo annotation to set the name of the column.

* Each table has a primary key that can be set using @PrimaryKey annotation.

 * You can use @Ignore annotation to ignore fields.

 * You can use full-text search to search for details in your database's tables. See implementation here

@AutoValue annotation can be used if there are two instances of an entity are equal.

 ## Define relationships between objects :
Room doesn't allow object references, but you can create embedded objects.
Use @Embedded annotation to represent an object that you'd like to divide into its subfields within a table.
Relations:
 1 -one-to-one: each instance of the parent entity corresponds to exactly one instance of the child entity, and vice-versa.
- 2-one-to-many: each instance of the parent entity corresponds to many instances of the child entity.
 - 3 - many-to-many: many instances of the parent entities correspond to many instances of the child entities and vice-versa.
 - @Relation annotation, parentColumn and entityColumn to set the relation between entities.


 * Accessing data using Room DAOs
 * DAO is used to ease the test of your app while you mock database.

  ## There are two types of DAO methods that define database interactions:

- 1 - Convenience methods: insert, update, and delete.
 - @Insert annotation used to declare methods that are inserting data into tables.
 - @Update annotation used to declare methods that are updating data into tables.
 - @Delete annotation used to declare methods that are deleting data into tables.
 - 2 - Query methods: write your own SQL query.
 - @Query annotation allows you to write SQL statements and expose them as DAO methods.

   
