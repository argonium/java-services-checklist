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
  * [Amazon Web Services](https://aws.amazon.com/)
  * [Google Cloud Platform](https://cloud.google.com/)
  * [MS Azure](https://azure.microsoft.com/)
  * [Digital Ocean](https://www.digitalocean.com/)
  * [Heroku](https://www.heroku.com/)
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
  * [FlatBuffers](https://google.github.io/flatbuffers/)
  * Message queues if no response is required
* Data pipeline
  * [Netflix Suro](https://github.com/Netflix/suro)
  * [Apache Spark](https://spark.apache.org/)
  * [Apache Kafka](https://kafka.apache.org/)
* Memory Allocators
  * [jemalloc](http://jemalloc.net/)
* RDBMS
  * [MySQL](https://www.mysql.com/)
  * [PostgreSQL](https://www.postgresql.org/)
  * [AWS Aurora](https://aws.amazon.com/rds/aurora/)
* SQL strategies
  * Sharding
  * Read replicas
* NoSQL
  * Key-Value (AWS DynamoDB, Riak)
  * Document (CouchDB)
  * Columnar (HBase, Cassandra)
  * Graph (Neo4J)
* OLAP
  * [AWS Redshift](https://aws.amazon.com/redshift/)
* Database versioning
  * [Flyway](https://flywaydb.org/)
  * [Liquibase](https://www.liquibase.org/)
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
  * [Redis](https://redis.io/)
  * [Memcached](https://memcached.org/)
  * [Varnish](https://varnish-cache.org/)
  * [Squid](http://www.squid-cache.org/)
* Text search
  * [Elastic](https://www.elastic.co/)
* Message queues
  * [Apache ActiveMQ](https://activemq.apache.org/)
  * [RabbitMQ](https://www.rabbitmq.com/)
  * [AWS SQS](https://aws.amazon.com/sqs/)
  * [AWS SNS](https://aws.amazon.com/sns/)
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
  * [Infer](https://fbinfer.com/)
  * [PMD](https://pmd.github.io/)
  * [jchord](https://bitbucket.org/psl-lab/jchord/src/master/)
  * [Findbugs](http://findbugs.sourceforge.net/)
  * [Checkstyle](https://checkstyle.sourceforge.io/)
* Code formatter
  * [Google Java Formatter](https://github.com/google/google-java-format)
* Metrics
  * [Spring Boot Actuator](https://docs.spring.io/spring-boot/docs/current/reference/html/production-ready-features.html)
  * [Micrometer](http://micrometer.io/)
  * [Dropwizard Metrics](https://metrics.dropwizard.io/)
* Service discovery
  * [Zuul](https://github.com/Netflix/zuul)
  * [Eureka](https://github.com/Netflix/eureka)
  * [Consul](https://www.consul.io/)
  * [Zookeeper](https://zookeeper.apache.org/)
* Stress testing
  * [Apache JMeter](https://jmeter.apache.org/)
  * [Siege](https://github.com/JoeDog/siege)
  * [Gatling](https://gatling.io/)
* Transaction log tailing
  * [Debezium](https://debezium.io/)
  * [LinkedIn Databus](https://github.com/linkedin/databus)
  * [DynamoDB streams](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.html)
* Storage
  * [AWS S3](https://aws.amazon.com/s3/)
* Serverless
  * [AWS Lambda](https://aws.amazon.com/lambda/)
* Proactive bug finding
  * [Chaos Monkey](https://github.com/Netflix/chaosmonkey)
  * [Resilience4J](https://github.com/resilience4j/resilience4j)
  * [Hystrix](https://github.com/Netflix/Hystrix)
  * [Arthas](https://github.com/alibaba/arthas)
* Profiling
  * [Async Profiler](https://github.com/jvm-profiling-tools/async-profiler)
  * [YourKit](https://www.yourkit.com/features/)
  * [VisualVM](https://visualvm.github.io/)
  * [JProfiler](https://www.ej-technologies.com/products/jprofiler/overview.html)
  * [NetBeans Profiler](https://profiler.netbeans.org/)
  * [Java Flight Recorder](https://docs.oracle.com/javacomponents/jmc-5-4/jfr-runtime-guide/about.htm)
  * [Java Mission Control](https://www.oracle.com/java/technologies/javase-overview.html)
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
* Enable compression for JSON responses

