## Overview: Saving data with Room
- Room provides an abstration layer over SQLite to allow fluent database access while harnessing the full power of SQLite
- cache relevant pieces of data so when the device cannot access the network the user can still browse that content while they are offline. synced back to the server after back online

3 major components in Room:
- Database: `@Database` abstract class that extends `RoomDatabase`, Include list of entities associatied with database withing annotation. abstract method that has 0 arguments and returns the class that is annotated with `@Dao`
- Entity: represents a table within the database
- DAO: contains the methods used for accessing the database

## Defining entities in Room
- de fine sets of related fields as *entities*. For each entity a table is created within the associated `Database`
- Room must have access either make a field public or you can provide a getter and setter for it.
- each entity must define at least 1 field as a primary key. all fields need the annotation `@PrimaryKey`
- default Room used the class name as the database table name.
- default column names uses the field names
-if entity inherits fields from a parent entity usually easiest to us the `ignoredColumns` property of the `@Entity` attribute

## Related entitited in Room
- Room does not allow entity objects to reference each other
- `@Embedded` to store composed columns separately in the table
- one-to-one: create a class for each entity. One must include a variable that is a reference to the primary key of the other entity. Create new data class each instance holds parent entity and corresponding instance of child entity. Add method `DAO` class that returns all instances of the data class that pairs parent and child entity.
- one-to-many: parent entity corresponds to zero or more instances of the child entity but each instance of child entity can only correspond to exactly one instance of the parent entity
- many-to-many: instances of the parent entity corresponds to zero or more instances of the child entity and vice-cersa
- nested relationships: between tables

## Accessing data with Room
- `Dao` objects form the main component of Room as each includes methods that offer obstract access to the app database. You can separate different components of you database architecture
- `@Insert` generates an implementation that inserts all parameters into the database in a single transation
- `Update` modifies a set of entities, given as parameters, in the database. Uses a query that matches against the primary key of each entity
- `Delete` removes a set of entities given as parameters from the database
- `@Query` allows you to perform read/write operations on a database
