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
* Legal concerns
  * GDPR
  * Data privacy laws
  * Right to be forgotten
* Risks

## Topics (with examples)
* Java version / JVM language
  * Java 8, 11
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
  * Spring
  * Spring Boot
  * Dropwizard
* Web servers
  * Apache Tomcat
  * Jetty
  * Glassfish
  * Undertow
  * Grizzly
* Reverse proxies
  * Apache
  * Nginx
* Communication between services
  * gRPC
  * HTTP
  * Protocol buffers
  * REST
  * GraphQL
  * WebSocket
  * STOMP
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
  * JMS (ActiveMQ)
  * AMQP (RabbitMQ)
  * AWS SQS
  * AWS SNS
  * SQS+SNS (fanout)
  * Akka
* Dependency management
  * Maven
  * Gradle
* CI/CD
  * Jenkins
  * CloudBees
  * CircleCI
* Static code analysis
  * Sonar
  * PMD
  * Findbugs
* Code formatter
  * Checkstyle
* Metrics
  * Spring Actuator
  * Dropwizard Metrics
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

