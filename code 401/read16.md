### Spring Security is a: 
* powerful and highly customizable authentication and access-control framework. It is the de-facto standard for securing Spring-based applications. Spring Security is a framework that focuses on providing both authentication and authorization to Java applications.

### Spring Security Architecture :
* Spring Security is a framework that enables a programmer to impose security restrictions to Spring-framework–based Web applications through JEE components. In short, it is a library that can be used, extended to customize as per the programmer's needsv
* Application security boils down to two more or less independent problems: authentication (who are you?) and authorization (what are you allowed to do?).
![Spring](https://www.techtalks.lk/assets/images/posts/1540960050)
![Spring](https://raw.githubusercontent.com/spring-guides/top-spring-security-architecture/master/images/authentication.png)
 
 #### Customizing Authentication Managers:
* Spring Security provides some configuration helpers to quickly get common authentication manager features set up in your application. The most commonly used helper is the AuthenticationManagerBuilder, which is great for setting up in-memory, JDBC, or LDAP user details or for adding a custom UserDetailsService

#### Web Security:
![Spring](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSITynFLL8-IMUGLdvo006aZLtPqKj2DTkznA&usqp=CAU)
* The client sends a request to the application, and the container decides which filters and which servlet apply to it based on the path of the request URI. At most, one servlet can handle a single request, but filters form a chain, so they are ordered. In fact, a filter can veto the rest of the chain if it wants to handle the request itself. A filter can also modify the request or the response used in the downstream filters and servlet. The order of the filter chain is very important, and Spring Boot manages it through two mechanisms: @Beans of type Filter can have an @Order or implement Ordered, and they can be part of a FilterRegistrationBean that itself has an order as part of its API. Some off-the-shelf filters define their own constants to help signal what order they like to be in relative to each other (for example, the SessionRepositoryFilter from Spring Session has a DEFAULT_ORDER of Integer.MIN_VALUE + 50, which tells us it likes to be early in the chain, but it does not rule out other filters coming before it).
