# xbird-boot

A sample project for Spring Boot.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/

## 1. System Requirements

Spring Boot 2.0.3.RELEASE requires Java 8 or 9 and Spring Framework 5.0.7.RELEASE or above. Explicit build support is provided for Maven 3.2+ and Gradle 4.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#getting-started-system-requirements

## 2. Spring Boot Starters

The starters contain a lot of the dependencies that you need to get a project up and running quickly and with a consistent, supported set of managed transitive dependencies.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#using-boot-starter

## 3. Auto-configuration

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#using-boot-auto-configuration

## 4. Developer Tools

Spring Boot includes an additional set of tools that can make the application development experience a little more pleasant. The spring-boot-devtools module can be included in any project to provide additional development-time features. 

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#using-boot-devtools

## 5. Your first SpringApplication

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-spring-application

- Customizing the Banner
- Application Events and Listeners
- Web Environment
- Accessing Application Arguments (ApplicationRunner or CommandLineRunner)

Application events are sent in the following order, as your application runs:

- ApplicationStartingEvent 
- ApplicationEnvironmentPreparedEvent 
- ApplicationPreparedEvent 
- ApplicationStartedEvent 
- ApplicationReadyEvent 
- ApplicationFailedEvent 

## 6. Externalized Configuration

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-external-config

- Configuring Random Values
- Application Property Files
- Using YAML Instead of Properties
- Type-safe Configuration Properties

## 7. Profiles

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-profiles

## 8. Logging

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-logging

- Logback Extensions

## 9. Developing Web Applications

Spring Boot is well suited for web application development. You can create a self-contained HTTP server by using embedded Tomcat, Jetty, Undertow, or Netty. Most web applications use the `spring-boot-starter-web` module to get up and running quickly. You can also choose to build reactive web applications by using the `spring-boot-starter-webflux` module.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-developing-web-applications

- Spring Web MVC
- Spring WebFlux
- JAX-RS and Jersey

## 10. Security

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-security

- MVC Security
- WebFlux Security
- OAuth2
- Actuator Security

## 11. Working with SQL Databases

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-sql

- Configure a DataSource
- Using JdbcTemplate
- JPA and “Spring Data”
- Using jOOQ

## 12. Working with NoSQL Technologies

Spring Data provides additional projects that help you access a variety of NoSQL technologies, including: MongoDB, Neo4J, Elasticsearch, Solr, Redis, Gemfire, Cassandra, Couchbase and LDAP. Spring Boot provides auto-configuration for Redis, MongoDB, Neo4j, Elasticsearch, Solr Cassandra, Couchbase, and LDAP. 

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-nosql

- Redis
- MongoDB
- Solr
- Elasticsearch
- Cassandra
- Couchbase
- LDAP
- InfluxDB

## 13. Caching

The Spring Framework provides support for transparently adding caching to an application. At its core, the abstraction applies caching to methods, thus reducing the number of executions based on the information available in the cache. The caching logic is applied transparently, without any interference to the invoker. Spring Boot auto-configures the cache infrastructure as long as caching support is enabled via the @EnableCaching annotation.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-caching

Supported Cache Providers:

- Generic
- JCache (JSR-107) (EhCache 3, Hazelcast, Infinispan, and others)
- EhCache 2.x
- Hazelcast
- Infinispan
- Couchbase
- Redis
- Caffeine
- Simple

## 14. Messaging

The Spring Framework provides extensive support for integrating with messaging systems, from simplified use of the JMS API using JmsTemplate to a complete infrastructure to receive messages asynchronously. Spring AMQP provides a similar feature set for the Advanced Message Queuing Protocol. Spring Boot also provides auto-configuration options for RabbitTemplate and RabbitMQ. Spring WebSocket natively includes support for STOMP messaging, and Spring Boot has support for that through starters and a small amount of auto-configuration. Spring Boot also has support for Apache Kafka.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-messaging

- JMS (ActiveMQ, Artemis)
- AMQP (RabbitMQ)
- Apache Kafka

## 15. Calling REST Services with RestTemplate

If you need to call remote REST services from your application, you can use the Spring Framework’s RestTemplate class. Since RestTemplate instances often need to be customized before being used, Spring Boot does not provide any single auto-configured RestTemplate bean. It does, however, auto-configure a RestTemplateBuilder, which can be used to create RestTemplate instances when needed. The auto-configured RestTemplateBuilder ensures that sensible HttpMessageConverters are applied to RestTemplate instances.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-resttemplate

## 16. Calling REST Services with WebClient

If you have Spring WebFlux on your classpath, you can also choose to use WebClient to call remote REST services. Compared to RestTemplate, this client has a more functional feel and is fully reactive. You can create your own client instance with the builder, WebClient.create().

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-webclient

## 17. Validation

The method validation feature supported by Bean Validation 1.1 is automatically enabled as long as a JSR-303 implementation (such as Hibernate validator) is on the classpath. This lets bean methods be annotated with javax.validation constraints on their parameters and/or on their return value. Target classes with such annotated methods need to be annotated with the @Validated annotation at the type level for their methods to be searched for inline constraint annotations.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-validation

## 18. Sending Email

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-email

## 19. Distributed Transactions with JTA

Spring Boot supports distributed JTA transactions across multiple XA resources by using either an Atomikos or Bitronix embedded transaction manager. JTA transactions are also supported when deploying to a suitable Java EE Application Server.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-jta

- Atomikos
- Bitronix
- Narayana
- Using a Java EE Managed Transaction Manager
- Mixing XA and Non-XA JMS Connections
- Supporting an Alternative Embedded Transaction Manager

## 20. Hazelcast

If Hazelcast is on the classpath and a suitable configuration is found, Spring Boot auto-configures a HazelcastInstance that you can inject in your application.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-hazelcast

## 21. Quartz Scheduler

Spring Boot offers several conveniences for working with the Quartz scheduler.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-quartz

## 22. Spring Integration

Spring Boot offers several conveniences for working with Spring Integration.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-integration

## 23. Spring Session

Spring Boot provides Spring Session auto-configuration for a wide range of data stores. When building a Servlet web application, the following stores can be auto-configured:

- JDBC
- Redis
- Hazelcast
- MongoDB

## 24. Monitoring and Management over JMX

Java Management Extensions (JMX) provide a standard mechanism to monitor and manage applications. By default, Spring Boot creates an MBeanServer bean with an ID of mbeanServer and exposes any of your beans that are annotated with Spring JMX annotations (@ManagedResource, @ManagedAttribute, or @ManagedOperation).

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-jmx

## 25. Testing

Spring Boot provides a number of utilities and annotations to help when testing your application. Test support is provided by two modules: spring-boot-test contains core items, and spring-boot-test-autoconfigure supports auto-configuration for tests.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-testing

- JUnit
- Spring Test
- AssertJ
- Hamcrest
- Mockito
- JSONassert
- JsonPath

## 26. WebSockets

Spring Boot provides WebSockets auto-configuration for embedded Tomcat 8.5, Jetty 9, and Undertow. If you deploy a war file to a standalone container, Spring Boot assumes that the container is responsible for the configuration of its WebSocket support.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-websockets

## 27. Web Services

Spring Boot provides Web Services auto-configuration so that all you must do is define your Endpoints.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-webservices

## 28. Creating Your Own Auto-configuration

If you work in a company that develops shared libraries, or if you work on an open-source or commercial library, you might want to develop your own auto-configuration. Auto-configuration classes can be bundled in external jars and still be picked-up by Spring Boot.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#boot-features-developing-auto-configuration

## 29. Spring Boot Actuator

Spring Boot includes a number of additional features to help you monitor and manage your application when you push it to production. You can choose to manage and monitor your application by using HTTP endpoints or with JMX. Auditing, health, and metrics gathering can also be automatically applied to your application.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#production-ready

- Endpoints
- Monitoring and Management over HTTP
- Monitoring and Management over JMX
- Loggers
- Metrics
- HTTP Tracing

## 30. Deploying Spring Boot Applications

Spring Boot’s flexible packaging options provide a great deal of choice when it comes to deploying your application. You can deploy Spring Boot applications to a variety of cloud platforms, to container images (such as Docker), or to virtual/real machines.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#deployment

- Cloud Foundry
- Heroku
- OpenShift
- AWS
- Google Cloud
- Installing Spring Boot Applications

## 31. Build tool plugins

Spring Boot provides build tool plugins for Maven and Gradle.

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#build-tool-plugins

## 32. ‘How-to’ guides

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#howto

## 33. Appendices

https://docs.spring.io/spring-boot/docs/2.0.3.RELEASE/reference/htmlsingle/#appendix

- Appendix A. Common application properties
- Appendix B. Configuration Metadata
- Appendix C. Auto-configuration classes
- Appendix D. Test auto-configuration annotations
- Appendix E. The Executable Jar Format
- Appendix F. Dependency versions

## 34. Spring Boot Admin

This community project provides an admin interface for Spring Boot applications.

https://github.com/codecentric/spring-boot-admin