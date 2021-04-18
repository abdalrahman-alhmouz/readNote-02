#### RequestMapping :
* Request Mapping Basics
In Spring MVC applications, the RequestDispatcher (Front Controller Below) servlet is responsible for routing incoming HTTP requests to handler methods of controllers.

When configuring Spring MVC, you need to specify the mappings between the requests and handler methods.
![spring](https://springframework.guru/wp-content/uploads/2017/09/mvc.png)

##### Accessing Data with JPA :
 * JPA (Java Persistence API): JPA is a specification. It is a collection of classes and methods to persistently store the vast amounts of data into a database. It provides common prototype and functionality to ORM tools. By implementing the same specifiation, all ORM tools (like Hibernate, TopLink..) follows the common standarts.
![spring](https://terasolunaorg.github.io/guideline/5.2.0.RELEASE/en/_images/dataaccess_jpa.png)
 * What is difference between CrudRepository and JpaRepository interfaces in Spring Data JPA?
 * CrudRepository provides CRUD functions. PagingAndSortingRepository provides methods to do pagination and sort records. JpaRepository provides JPA related methods such as flushing the persistence context and delete records in a batch.٢٣‏/٠٨‏/٢٠١٩
![crude](https://1.bp.blogspot.com/-Hp5KPW5F_zc/XvP_DDboR-I/AAAAAAAAOj8/j28IVURGB4wJ1-ymh1ThNvZOaLCjZRahwCK4BGAsYHg/s583/CrudRepositoryVsJpaRepo.png)

