#### Working with Relationships in Spring Data REST:
* A one-to-many relationship is defined using the @OneToMany and @ManyToOne annotations and can have the optional @RestResource annotation to customize the association resource.
![related](https://i.stack.imgur.com/axCR9.png)




### Baeldung: Spring Integration Testing:
* Integration testing plays an important role in the application development cycle by verifying the end-to-end behavior of a system.

* Several Maven dependencies are required for running the integration tests we'll use in this article. First and foremost, we'll need the latest junit-jupiter-engine, junit-jupiter-api, and Spring test dependencies:

* Enable Spring in Tests with JUnit 5 :
* ![spring](https://image.slidesharecdn.com/integrationtestingformicroserviceswithspringbootcampv1-180305091229/95/integration-testing-for-microservices-with-spring-boot-12-638.jpg?cb=1520241277)
JUnit 5 defines an extension interface through which classes can integrate with the JUnit test.

We can enable this extension by adding the @ExtendWith annotation to our test classes and specifying the extension class to load. To run the Spring test, we use SpringExtension.class.

We also need the @ContextConfiguration annotation to load the context configuration and bootstrap the context that our test will use.
* Finally, we also annotate the test with @WebAppConfiguration, which will load the web application context.


