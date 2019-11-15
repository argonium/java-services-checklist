# Java Back-End Development

## Prerequisites

We need to first assess the following information:

* What assumptions are we making for the software?
* Who is our audience?
* What is the goal of the software?
* What are the high-level requirements?
* What are the high-level non-requirements?
* What are the security requirements?
* What are the external dependencies?
* What are the non-functional requirements?
  * Performance
  * Scalability
  * Availability
  * Testability
  * Code quality
* Accessibility requirements
  * ADA
  * Section 508
* Legal concerns and regulations
  * PCI (credit card data)
  * SOX (financial)
  * HIPAA (health care)
  * SAS-70, SSAE 16, AT801 (auditing)
  * GDPR
  * California Consumer Privacy Act
  * Right to be forgotten
* Risks

## Topics (with examples)
* Java version / JVM language
  * Java 8, 12
  * Scala, Clojure, Kotlin
  * Do we need long-term support?
  * If using Docker, fewer restrictions on the language
* Architecture
  * Monolith
  * Microservices
  * Lambda / serverless
  * Multiple (microservices + lambda)
  * Migration (monolith -> microservices)
* Hosting provider
  * Amazon Web Services
  * Google Cloud Platform
  * MS Azure
  * Digital Ocean
  * Heroku
* Framework
  * [Spring](https://spring.io/)
  * [Spring Boot](https://spring.io/projects/spring-boot)
  * [Dropwizard](https://www.dropwizard.io/)
  * [Helidon](https://helidon.io/)
  * [Micronaut](https://micronaut.io/)
  * [Proteus](https://github.com/noboomu/proteus)
  * [Rapidoid](https://www.rapidoid.org/)
  * [Jooby](https://jooby.org/)
* Web servers
  * [Apache Tomcat](http://tomcat.apache.org/)
  * [Jetty](https://www.eclipse.org/jetty/)
  * [Glassfish](https://www.oracle.com/technetwork/middleware/glassfish/overview/index.html)
  * [Undertow](http://undertow.io/)
  * [Grizzly](https://javaee.github.io/grizzly/)
  * [JLHTTP](https://www.freeutils.net/source/jlhttp/)
  * [Vert.x](https://vertx.io/)
* Reverse proxies
  * [Apache](https://httpd.apache.org/)
  * [Nginx](https://www.nginx.com/)
* Communication between services
  * [gRPC](https://grpc.io/)
  * [Cap'n Proto](https://capnproto.org/)
  * [Protocol buffers](https://developers.google.com/protocol-buffers)
  * [REST](https://restfulapi.net/)
  * [GraphQL](https://graphql.org/)
  * [WebSocket](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API)
  * [STOMP](https://stomp.github.io/)
  * Message queues if no response is required
* Data pipeline
  * Netflix Suro
  * Apache Spark
  * Apache Kafka
* RDBMS
  * MySQL
  * PostgreSQL
  * AWS Aurora
* SQL strategies
  * Sharding
  * Read replicas
* NoSQL
  * Key-Value (AWS DynamoDB, Riak)
  * Document (CouchDB)
  * Columnar (HBase, Cassandra)
  * Graph (Neo4J)
* OLAP
  * AWS Redshift
* Database versioning
  * Flyway
  * Liquibase
* Containerization
  * Docker
  * Kubernetes
  * AWS Fargate
* JDBC Connection Pooling
  * [Apache Commons DBCP](https://commons.apache.org/proper/commons-dbcp/)
  * [HikariCP](https://brettwooldridge.github.io/HikariCP/)
  * [C3P0](https://www.mchange.com/projects/c3p0/)
* Spring REST Specs
  * RAML
  * Swagger
  * Spring REST Docs
* Security
  * Spring Security
  * OpenID
  * LDAP
  * AD
  * OAuth
  * JWT
  * SSO
  * Session cookies
* Unit tests
  * JUnit
  * TestNG
  * Spock
  * Mutation testing
* Mocking
  * Mockito
  * PowerMock
  * Wiremock (mock endpoints)
  * Mountebank
  * Pacto
* Integration tests
  * EasyB
  * JBehave
  * Selenium
  * Cucumber
  * Postman Collections
  * Protractor
  * Pact
* Code coverage
  * JCov
  * JaCoCo
  * Clover
  * OpenClover
* Application Performance Monitoring
  * NewRelic
  * Pingdom
  * DataDog
  * AppDynamics
  * Pinpoint
* System monitoring
  * Grafana
  * Graphite
  * Prometheus
  * AWS CloudWatch
  * StatsD
  * Nagios
* Distributed tracing
  * Zipkin
  * Spring Cloud Sleuth
  * Dapper
  * HTrace
  * [Jaeger](https://www.jaegertracing.io/)
* Data Access Layer
  * Hibernate
  * Spring Data
  * JDBC
* Logging
  * Log4j
  * Logback
  * Slf4j
  * Structured logging
* Logging collation
  * Logstash
  * Splunk
  * AWS Cloudtrail
  * LogRocket
* Logging visualization
  * ELK
* Caching
  * Redis
  * Memcached
  * Varnish
  * Squid
* Text search
  * Elastic
* Message queues
  * [Apache ActiveMQ](https://activemq.apache.org/)
  * [RabbitMQ](https://www.rabbitmq.com/)
  * AWS SQS
  * AWS SNS
  * SQS+SNS (fanout)
  * [Akka](https://akka.io/)
  * [Apache Pulsar](https://pulsar.apache.org/)
* Dependency management
  * [Apache Maven](https://maven.apache.org/)
  * [Gradle](https://gradle.org/)
* CI/CD
  * [Jenkins](https://jenkins.io/)
  * [CloudBees](https://www.cloudbees.com/)
  * [CircleCI](https://circleci.com/)
* Static code analysis
  * [Sonar](https://www.sonarqube.org/)
  * [SpotBugs](https://spotbugs.github.io/)
  * [PMD](https://pmd.github.io/)
  * [Findbugs](http://findbugs.sourceforge.net/)
  * [Checkstyle](https://checkstyle.sourceforge.io/)
* Code formatter
  * [Google Java Formatter](https://github.com/google/google-java-format)
* Metrics
  * [Spring Boot Actuator](https://docs.spring.io/spring-boot/docs/current/reference/html/production-ready-features.html)
  * [Micrometer](http://micrometer.io/)
  * [Dropwizard Metrics](https://metrics.dropwizard.io/)
* Service discovery
  * Zuul
  * Eureka
  * Consul
  * Zookeeper
* Stress testing
  * Apache JMeter
  * Siege
  * Gatling
* Transaction log tailing
  * Debezium
  * LinkedIn Databus
  * DynamoDB streams
* Storage
  * AWS S3
* Serverless
  * AWS Lambda
* Proactive bug finding
  * Circuit Breaker
  * Chaos Monkey
  * Resilience4J
  * Hystrix
* Fuzzing
  * ClusterFuzz
  * American Fuzzy Lop
* Configuration management
  * Hashicorp Vault
  * Confidant (Lyft)
  * AWS Parameter Store
* Usage reports
  * Google Analytics
* Artifact management
  * Artifactory
* HTTP sniffers
  * HTTPScoop
  * Fiddler
  * Charles
* Java code generators
  * Lombok
  * AutoValue
* Standalone REST clients
  * Postman
  * Advanced REST Client
  * Paw
  * Insomnia

## Tips

* If using Spring, start with Spring Initializr
* If using AWS Lambda, weigh the usage requirements with the budget
* Design for mobile first
* Consider the BFF design pattern for different clients (mobile, web)
* Consider the Saga pattern for failure recovery
* Avoid premature optimization
* Controllers should not throw exceptions
* ORMs are handy for POCs or if the SQL design changes frequently, but not for performance
* Use REST Standards
  * POST (create)
  * PUT (update)
  * GET (no side effects)
  * DELETE
* Deployments should be a one-step process (blue-green deployments)
* Writing MBeans for JConsole can help with gathering runtime data

