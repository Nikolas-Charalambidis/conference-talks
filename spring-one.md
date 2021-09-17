# [Spring One](https://springone.io/)

- All sessions for free and online since the 7th of September 2021

| Session                                                                                           | Tags                          | Length | Track                        |
|---------------------------------------------------------------------------------------------------|-------------------------------|--------|------------------------------|
| [How To Be a Java Automated Testing Superstar](#how-to-be-a-java-automated-testing-superstar)     | #architecture #testing        | 26:24  | Architecture                 |
| [Deploy Code into Production Faster on Kubernetes](#deploy-code-into-production-faster-on-kubernetes) | #devops #cloud #native #microservices | 27:31 | Cloud Native Platforms |
| [Modern Application Configuration in Kubernetes](#modern-application-configuration-in-kubernetes) | #devops #kubernetes #spring #cloud | 26:49 | Architecture             |
| [You Can Be Cloud Native, Too](#you-can-be-cloud-native-too)                                      | #cloud #native                | 27:00  | Beginner-Friendly Spring     |
| [A Developer’s Introduction to Containers](#a-developers-introduction-to-containers)              | #containers #devops           | 26:15  | Cloud Native Platforms       |
| [Building Fast and Scalable Persistence Layers with Spring Data JPA](#building-fast-and-scalable-persistence-layers-with-spring-data-jpa) | #spring #jpa #hibernate | 54:50 | Intermediate/Advanced Spring |
| [Packaging and Distributing Applications for Kubernetes](#packaging-and-distributing-applications-for-kubernetes) | #containers #devops           | 24:55  | Architecture |
| [From Spring Framework 5.3 to 6.0](#from-spring-framework-53-to-60)                               | #java #spring #jakarta        | 25:34  | Intermediate/Advanced Spring |
| [Spring Security 5.5 From Taxi to Takeoff](#spring-security-55-from-taxi-to-takeoff)              | #spring #security             | 51:05  | Beginner-Friendly Spring     |
| [Test-Driven Security](#test-driven-security)                                                     | #spring #security #test       | 22:25  | Intermediate/Advanced Spring |
| [Code Wars: Database Decisions for Application Development](#code-wars-database-decisions-for-application-development) | #spring #security #test | 51:14 | Beginner-Friendly Spring |
| [Spring Data JDBC: Beyond the Obvious](#spring-data-jdbc-beyond-the-obvious)                      | #spring #data #jdbc           | 52:39  | Intermediate/Advanced Spring |
| [Microservices Testing at Scale](#microservices-testing-at-scale)                                 | #microservice #test           | 22:58  | Architecture                 |
| [A Spring Data’s Guide to Persistence](#a-spring-datas-guide-to-persistence)                      | #spring #data                 | 53:54  | Beginner-Friendly Spring     |
| [Live Coding Spring Data Queries to the End of the Persistence Universe](#live-coding-spring-data-queries-to-the-end-of-the-persistence-universe) | #spring #data | 26:11 | Beginner-Friendly Spring |
| [Leap Ahead with Redis 6.2](#leap-ahead-with-redis-62)                                            | #spring #data #redis          | 55:32  | Beginner-Friendly Spring     |
| [Winning the Lottery with Spring: A Microservices Case Study for the Dutch Lotteries](#winning-the-lottery-with-spring-a-microservices-case-study-for-the-dutch-lotteries) | #spring #microservices | 27:12 | Architecture |
| [Live Coding Spring, Kafka, & Elasticsearch: Personalized Search Results on Ranking and User Profile](#live-coding-spring-kafka--elasticsearch-personalized-search-results-on-ranking-and-user-profile) | #spring #elasticsearch | 26:42 | Architecture |
| [Debugging Complex Issues in Web Applications](#debugging-complex-issues-in-web-applications)     | #spring #tomcat               | 51:15  | Intermediate/Advanced Spring |
| [Spring Boot—Production Boost](#spring-bootproduction-boost)                                      | #spring #kubernetes           | 26:09  | Beginner-Friendly Spring     |
| [How to Use KPIs in an Agile Delivery Environment](#how-to-use-kpis-in-an-agile-delivery-environment) | #agile #project #management #kpi | 24:15 | Agile Leadership       |
| [Why Every Software Team Should Have a Designer](#why-every-software-team-should-have-a-designer) | #agile #project #management   | 23:24  | Agile Leadership             |

_____

## [How To Be a Java Automated Testing Superstar](https://springone.io/2021/sessions/how-to-be-a-java-automated-testing-superstar)
> "Write automated tests until they give me the confidence to deploy PROD without manual intervention."
- Length 26:24, watched on 2021-09-07, **#architecture #test**
- Billy Korando as Java Developer Advocate, Oracle
- Track: Architecture

### Keynotes
- Automated tests should be human-readable and treated as same as the production code. They are repeatable and auditable.
- **Dependency iceberg** says that our code is just a tip of all the code the application runs on. The dependencies are below.
  - Most of the code are dependencies, feature and performance enhancements (Spring libraries, JSON/XML mappers, ORM implementation, servlets, etc.), and security patches.
  - We cannot rely 100% on it, especially if we use the last stable versions. On the other hand, old versions have security flaws (Struts).
- How many automated tests should I write? Whatever gives me the confidence to deploy PROD without manual intervention (i.e. code coverage is just informative).
- Manual testing is still needed but it is exploratory testing.

### Rating ⭐⭐⭐⭐☆
- ✅ Theoretical aspects and importance of testing, best-practices of unit testing.
- ⛔ Too short (not the speaker's fault), code examples weren't that impressive, no mention about [BDD](https://en.wikipedia.org/wiki/Behavior-driven_development) approach.

_____

## [Deploy Code into Production Faster on Kubernetes](https://springone.io/2021/sessions/modern-application-configuration-in-kubernetes)
> "Developer experience on DIY platforms is lacking."
- Length 27:31, watched on 2021-09-07, **#devops #cloud #native #microservices**
- Valentina Alaria as Director Product Management, VMware
- Track: Cloud Native Platforms

### Keynotes
- Most of Kubernetes offerings are delivered as a bag of parts:
  - 63 % of organizations, if use K8S, use as internal platforms or build internal platforms.
  - 94 % of organizations, if use K8S, building internal platforms use more than one platform.
  - 58 % of organizations agree that architectural decision making has gotten harder.
- Developer experience on DIY platforms is lacking. Developers must still maintain containers, configure containers run through multiple layers of YAML, manage IT and security aspects.
- Importance lies in tooling to help developers: leverage automatized DevOps practices, enforce organizational best-practices, app-aware platform, preconfigured templates by Ops.

### Rating ⭐⭐☆☆☆
- ✅ Beginner-friendly introduction, on-spot developer concerns identification.
- ⛔ The structure doesn't match the agenda in the introduction and a bit chaotic, rather Tanzu platform promotion, lacking expected pure K8S tips

_____

## [Modern Application Configuration in Kubernetes](https://springone.io/2021/sessions/modern-application-configuration-in-kubernetes)
> "Spring Cloud Config vs. K8S Config-maps and secrets."
- Length 26:49, watched on 2021-09-07, **#devops #kubernetes #spring #cloud**
- Craig Walls as Engineer, VMware
- Track: Architecture

### Keynotes
- Spring applications environment configuration is based on Spring Environment Abstraction as of Spring 3.1 (`application.properties`, `application.yml`, command-args, JVM system properties...). 
- They can be in the filesystem and are very difficult to audit and manage across multiple applications and instances.
  - Spring Environment Abstraction is extensible and has a solution for versioned (Git, Vault, DB, CredHub...), audited (git log) and centralized configuration - Spring Cloud Config Server
  - Such configuration must be read from the server and merged into Environment - Spring Cloud Config Server client library
  - Although Spring Config Server/Client can run on K8S, it must be merged into Resources, that are K8S native, like config-maps and secrets - Tenzu
- **Spring Cloud Config:** Central management of properties, can be versioned, can be audited, HTTP-based property consumption, probably should be secured, requires client-size library or code
- **K8S Config-maps and secrets:** Doesn't require special client code, K8S-native, not centrally managed, versioning/auditing is not built-in, can leverage K8S-native security
 
### Rating ⭐⭐⭐⭐⭐
- ✅ Very catchy speech, an excellent introduction into the environment properties management problem and comparison of approaches
- ⛔ The speaker has only one session

_____

## [You Can Be Cloud Native, Too](https://springone.io/2021/sessions/you-can-be-cloud-native-too)
- Length 27:00, watched on 2021-09-07, **#cloud #native**
- Hananiel Sarella as Software Engineer, VMware
- Track: Beginner-Friendly Spring

### Keynotes
- Pros: Microservice architecture provides easy to maintain, test, and deploy services, teams can be scaled, polyglot-friendly, 
- Cons: Distribute systems are rather complex and interaction is difficult to test, memory consumption and overhead
- Cloud-native patterns: Consistent management, run everywhere, secure, seamlessly adopt new environments, distributed systems patterns and abstractions
- Steeltoe Project introduction on top of .NET foundation enables building production-grade and cloud-native microsystems in a simplified way quick to stand up
  - Scalability (service discovery, configuration providers), Resilience (circuit breaker, bulkhead, client-side load balancing), Ease of Use (initializer, autoconfiguration, platform providers and connectors such as DB, MQ, OAuth), Observability (management endpoints, dynamic logging, distributed tracing, metrics), Security (SSO, JWT auth, certificates), Messaging (stream processing)

### Rating ⭐⭐⭐☆☆
- ✅ Broad overview of microservice architecture facilities and difficulties
- ⛔ Missing introduction into cloud-native concepts since this is marked as beginner-friendly, too many buzzwords, .NET examples, I can't extract the gist or quote of the talk into the header

_____

## [A Developer’s Introduction to Containers](https://springone.io/2021/sessions/a-developers-introduction-to-containers)
> "Container is process isolation."
- Length 26:15, watched on 2021-09-08, **#containers #devops**
- Nigel Brown as Senior Open Source Community Manager, VMware
- Track: Cloud Native Platforms

### Keynotes
- Container is a process or group of processes running in isolation, it is great for portability and security
- The way of achieving the process isolation is by leveraging several features of the Linux kernel:
- **[Namespaces](https://en.wikipedia.org/wiki/Linux_namespaces)** 
  - They wrap global system resources in an abstraction that makes it appear to the process within the namespace, that they have their own instance of the resource.
  - Process *one* and *zero* are typically reserved for what it takes to initialize our OS. In a container, typically, the application is running an application with process id *one* That's a whole instance of the process id counter that's working inside of the container that is different from what's happening outside and that's achieved by having a separate namespace from within which to work.
- **[cgroups](https://en.wikipedia.org/wiki/Cgroups)**
  - Control groups allow processes to be organized into hierarchical groups whose usage of various types of resources can be then limited and monitored.
  - Basically, it allows assigning a maximum number of resources each group can allocate to ensure your critical system processes always have the resources they need to run.  

### Rating ⭐⭐⭐⭐⭐
- ✅ Excellent explanation of the container and Linux kernel concepts, simple but nice workshop
- ⛔ Slides would be better to support the ideas at the beginning

_____

## [Building Fast and Scalable Persistence Layers with Spring Data JPA](https://springone.io/2021/sessions/fast-and-scalable-persistence-layers-with-spring-data-jpa)
> "Favour DTO interfaces projections without advanced techniques (SpEL, nested associations) for read-operations over managed entities."
- Length 54:50, watched on 2021-09-08, **#spring #jpa #hibernate**
- Thorben Janssen as Freelancer, Self-employed
- Track: Intermediate/Advanced Spring

### Keynotes
- Hibernate statistics: Properties `hibernate.generate_statistics=true`, `hibernate.session.events.log.LOG_QUERIES_SLOWER+THAN_MS=3` and logging `org.hibernate.stats=DEBUG` (for DEV purposes).
- **Assciation management**
  - `FetchType` recommendtion:
    - To-many relationships: Stick to the default mapping `FetchType.LAZY` and use fetching for specific queries if required.
    - To-one relationships: Check existing mappings individually and use `FetchType.LAZY` for new ones.
  - N+1 problem that lazy fetching introduces: 
    - Fetch all required entities with one query using Fetch Joins (`JOIN FETCH` in `@Query` or Entity Graphs (@NamedEntityGraph` and `@EntityGraph`)
    - Beware of left-joining as the complexity of the queue raises and it becomes slower. Although it's recommended to not join more than one association, it also depends on whether it contains 3 or thousands of rows.
  - Hibernate and many-to-many:
    - Hibernate handles `List` inefficiently (it removes all associations and adds remaining ones) so is better to use `Set`.
- **Projections** help to fine-tune the data that you actually need, so less data is selected from the database
  - Write-operations: 
    - Entities are managed by the current persistence context, which means at the end of the transaction the managed entity is updated in the database through queries
  - Read-operations: They don't need lifecycle management overhead (no `INSERT`/`UPDATE`/`DELETE`).
    - Scalar values are object arrays (`Obejct[]`) and need to remember the order in the `SELECT` clause.
    - DTO classes (without `@Entity` for pure JPA) and interfaces with matching getter methods (easier, Spring Data JPA generates a class based on the definition) are preferred over scalar values
- **Advanced DTO projections pitfalls** 
  - Nested associations such as a getter returning `List<ClientDtoProjecion>` on an interface-based DTO projection actually defies all the benefits of the DTO projections introduced earlier
  - SpEL such as returning first and last name together using `@Value("#{target.lastName + ', ' + target.firstName}") over a getter actuall selects a whole entity and it is better to use a `default` interface method performing the concatenation instead and preserve he benefits of DTO proections
- **Caching**
  - 1st level cache: 
    - Each Hibernate session has 1st level cache assuring we have only one object representation of each record in the database within each session, but it is useless performance-wise when each user has their own session.
  - 2nd level cache:
    - It is a session independent entity store containing entity objects and is used whenever an entity is found by its primary key (or if associations are traversed), but it creates some additional problems because now this external cache is needed to keep in sync (check first) that creates a small overhead and it's needed to compensate with a higher number of hits (rule of thumb is at least 9-10 reads per 1 write operation).
    - It needs to be activated in properties with a specific cache mode where `ENABLE_SELECTIVE` and `DISABLE_SELECTIVE` is recommended over `ALL`/`NONE`/`UNSPECIFIED` and managed through `@Cacheable` annotation on the repository class/method or entity class level.
    - Tip: Place `@Cache(use = CacheCocurrencyStrategy.TRANSACTIONAL) over many-to-many associations and all associations on entities that don't map the foreign key column, because in these cases Hibernate doesn't cache the *association* between these two objects but *only* the objects themselves.

### Rating ⭐⭐⭐⭐⭐
- ✅ Practical workshop with an on-spot set of tips for working with Hibernate and Spring Data JPA effectively
- ⛔ An alternative to SpEL was introduced but not to the nested association within advanced DTO projection

_____

## [Packaging and Distributing Applications for Kubernetes](https://springone.io/2021/sessions/packaging-and-distributing-applications-for-kubernetes)
> "Carvel is a composable Kubernetes tool suite."
- Length 24:55, watched on 2021-09-08, **#devops #kubernetes**
- Ian Zink as Staff Software Engineer, VMware
- Nitasha Verma as Solutions Engineer, VMware
- Track: Architecture

### Keynotes
- Relocating K8S configurations and containers in the hands of their customers as a secure, consistent, and unified distribution within the framework of their existing ecosystem is clumsy.
- Application lifecycle (packagin and deployment on K8S): Author Configuration -> Package and Distribution -> Customizing Configuration -> Deploy to Cluster.
- Carvel is a composable Kubernetes tool suite, which provides a set of reliable, single-purpose, composable tools that aid in your application building, configuration, and deployment to Kubernetes. Basic tools:
  - `ytt`: Template and overlay K8S via YAML structures.
  - `kbld`: Build or reference container images in K8S configuration in an immutable way.
  - `kapp`: Install, upgrade, and delete multiple K8S resources as one application.
  - `imgpkg`: Bundle and relocate application configuration (with images) via Docker registers.

### Rating ⭐⭐⭐☆☆
- ✅ Well structured presentation with a demo, they were able to find a workaround for an unexpected error they faced during the demo
- ⛔ Overly abstract terms (configuration, bundle, registers...) and commands in the demo were insufficiently described

______

## [From Spring Framework 5.3 to 6.0](https://springone.io/2021/sessions/from-spring-framework-5-3-to-6-0)
> "Spring Framework **5.3.x** remains in active development and Spring Framework **6.0** will be the beginning of a new generation."
- Length 25:34, watched on 2021-09-08, **#java #spring #jakarta**
- Juergen Hoeller as Spring Framework Project Lead, VMware
- Track: Intermediate/Advanced Spring

### Keynotes
- Spring Framework **5.3.x**:
  - Java 17 support against a Java 8 baseline, support in Spring Boot 2.6 as of November 2021.
  - Java EE 8 focus agasint a Java EE 7 baseline.
- Spring Framework **6.0**:
  - Development branch (main) will be established in mid of September, milestone phase at the end of 2021 (`6.0.M1` version), release candidate phase in mid-2022 (`6.0.RC1`). and `6.0` GA in October 2022.
  - Release cadence is yet undecided, might follow Boot's half-year rhythm.
  - Spring Native initiative moves into Spring proper, AOT processed metadata for regular JVM deployment as well.
  - Introduces core abstractions
- Spring Boot 2.7 as of May 2022.
- Spring Boot 3.0 introduces starter for native applications, build plugins and support for specific GraalVM versions, and auto-configuring the observability backend
- Java 17 enforces illegal access rules, no general escape hatch anymore.

### Rating ⭐⭐⭐☆☆
- ✅ Interesting overview of upcoming versions and timing
- ⛔ Missing examples of existing problems that new features would resolve, 60% of the time is rather focused on terms than features

_____

## [Spring Security 5.5 From Taxi to Takeoff](https://springone.io/2021/sessions/spring-security-5-5)
> "Spring Security integrates the Spring Native for all of its authentication mechanism and all of its authorization models."
- Length 51:05, watched on 2021-09-08, **#spring #security**
- Josh Cummings as Software Engineer, VMware
- Marcus Da Coregio as Software Engineer, VMware
- Steve Riesenberg as Software Engineer, VMware
- Track: Beginner-Friendly Spring

### Keynotes
- **Secured by default first principle**
  - `spring-boot-starter-security` present on classpath means is that every endpoint either user-generated or Spring Boot-generated (`GET /error`) requires Basic authentication with `user` username and randomly generated password printed into the console (protection if Spring profile is not changed by mistake).
  - The random password is generated until the default security configuration is overwritten (`UserDetailsService` bean). 
- **Personalize the application to the logged user**
  - Thread local `SecurityContextHolder` gives access for the application available anywhere on the current thread-bound in a servlet application to the current request.
  - `SecurityContextHolder.getContext().getAuthentication()` gives some of that information about the currently logged-in user, but there are little difficulties with testing of this code because it is needed to mock out the thread-local pattern, security context, and authentication, so method injection is preferred (`List<Flight> getFights(Authentication auth)`).
- **Authorization of a certain endpoint**
  - Some endpoints must be restricted to certain users, so it is needed to define either *roles* or *authorities* to them in `UserDetailsService` bean and map endpoints to the authority through `SecurityFilterChain` bean (`.httpBasic(Customizer.withDefaults())` must be added though).
  - It is needed to provide CSRF token to pass through the `CsrfFilter` to prevent [cross-site request forgery](https://owasp.org/www-community/attacks/csrf), ex. `.csrf((csrf) -> csrf.csrfTokenRepository(CookieCsrfTokenRepository.withHttpOnlyFalse())` and defining `CorsConfigurationSource` bean - The preflight (`OPTIONS` HTTP method) request conains the CORS headers on response and in the request to `POST`/`PUT` is present header `Access-Control-Allow-*`, and `Cookie` with the `XSRF-TOKEN` token and `X-XSRF-TOKEN` header itself together called *double submitting cookie*. 
  - It is needed to manage CORS to allow call endpoints from the endpoint using `.cors(Customizer.withDefaults())`.
- **Insecure direct object reference vulnerability**
  - Secure wildcard endpoints such as `PUT /{flightId}/taxi` are vulnerable as it is not checked if the object to be modified is compliant with the current authentication.
  - It is not preferred to weave the authentication behavior into the business logic and use more declarative security patterns using the domain-specific language (DSL), ex. `@PostAuthorizate("returnObject?.pilotId == authentication.name")` for outputs or `@PreAuthorize` for inputs are both compliant with the Spring transaction management and upon exception thrown by this construct any kind of change to the database will be rolled back - to get Spring Security to honor these annotations, `@EnableGlobalMethodSecurity(prePostEnabled = true)` is required.
- **Externalize the authorizaion** creating a `@Component` impementing `AuthorizationManager<RequestAuthorizationContext>` delegating check to `RequestMatcherDelegatingAuthorizationManager`, using `@EventListener` to apply the rules read once from the database and applying to `SecurityFilterChain`.
- Spring Security integrates the Spring Native for all of its authentication mechanisms and all of its authorization models (except SAML).
- **Speed it up** from `200ms` to `2ms`
  - Basic authentication means the credentials are sent every single time and the password needs to be hashed every time and compared against what is in the user store (especial using BCrypt algorithm that adds some amount of time) - switch over to a different authentication scheme, Bearer tokens as JWT tokens, bringing in the `spring-bot-starter-oauth2-resource-server` dependency (the resource server part allows to perform decoding tokens and using them as authentication mechanism) and removing `.httpBasic(Customizer.withDefaults())` with `.csrf(..)` and adding `.oauth2ResourceServer(OAuth2ResourcesServerConfigurer::jwt)` that also configures JWT out of the box.
  - OAuth2 authorization server is needed to be added to mint the tokens and to give some secure keys to verify a signature on them through properties `spring.security.oauth2.resourceserver.jwt.jwk-set-uri` and `spring.security.oauth2.resourceserver.jwt.issuer-uri`.
  - Finally, it is needed to define bean `JwtAuthenticationConverter` to make sure that the stored authorities in the database come back and match when a token is decoded.
- **Debugging** Spring Security application is easy through `org.springframework.security=TRACE` logging level.
  - `FilterChainProxy` is the entry point and a first place that Spring-secured interceptor requests fall in and then come to the `SecurityFilterChain` and to the further filters that either call the next filter or terminate the request by interrupting ~ [Chain of Responsibility](https://en.wikipedia.org/wiki/Chain-of-responsibility_pattern) design pattern.
- **Testing** is also easy in `@SpringBootTest` and `@AutoConfigureMockMvc` using `@WithMockUser(username, authorities)` annotation and static helpers in `org.springframework.security.test.**` packages. 

### Rating ⭐⭐⭐⭐⭐
- ✅ Well-prepared, exhaustive and entertaining role-played scenario securing application step-by-step, key takeaways summary at the end
- ⛔ CSRF demo showing requests and responses is difficult to follow and could be explained better

______

## [Test-Driven Security](https://springone.io/2021/sessions/test-driven-security)
> "Feature development is guided by writing failing tests first and then write the minimal amount of code necessary to make a test pass."
- Length 22:25, watched on 2021-09-08, **#spring #security #test**
- Eleftheria Stein-Kousathana as Software Engineer, VMware
- Track: Intermediate/Advanced Spring

### Keynotes
- Dependency `org.springframework.security:spring-security-test` brings helpers in `org.springframework.security.test.**` packages and more:
  - `mockMvc = MockMvcBuilders.webAppContextSetup(context).apply(springSecurity()).build();` using autowired `WebApplicationContext`
  - `get("/greeting").with(user("Ria")).with(csrf()).andExpect(..)..`
- `String greeting(@AuthenticationPrincipal(expression = "username") String username)` injects in the currently logged user's username and `String greeting(@AuthenticationPrincipal CustomUser user)` to injects in a subtype of `UserDetails`.

### Rating ⭐⭐⭐⭐⭐
- ✅ Simple introduction to Spring security testing, TDD approach, OWASP mentioned
- ⛔ Session labeled as *Intermediate/Advanced Spring* track should include a sample of OAuth2 testing, quite a short talk (22 mins of 30 mins available, other speakers use around 25-26 minutes) 

_____

## [Code Wars: Database Decisions for Application Development](https://springone.io/2021/sessions/database-decisions-for-application-development)
> ""
- Length 51:14, watched on 2021-09-09, **#spring #security #test**
- Jennifer Reif as Developer Relations Engineer, Neo4j
- Track: Beginner-Friendly Spring

### Keynotes
- Databases
  - In long-term is the right tool for the right job worth for future maintenance/improvement efforts
  - In the short-term forces data into the unnatural format, confuses data model, and delegates business questions to complex queries, data storage can impact application development 
- Spring Data provides annotation-based mapping for POJO domain classes, repository support via interfaces, and DSL queries for each datastore
- MariaDB as an example of relational database model through Spring Data JPA dependency
  - `orders(orderId, orderDate)`, `products(productId, productName)` and `orderProducts(quantity, unitPrice)` tables representing M:N relationship between `orders` and `products`.
  - The concepts are `@Entity`, `@Table`, `@Id`, `@Column`, `@OneToOne`/`@OneToMany`/`@ManyToOne`/`@ManyToMany`, `@JoinColumn` JPA (`javax.persistence`/`jakarta.persistence`) and Spring Data annotations and `CrudRepository<E, ID>` interface with `@Query` annotation using JQL/HQL as a domain-specific language for querying from the database.
  - Relevant properties are `spring.dtasource.**` and `spring.jpa.**`
- MongoDB as an example of document database model through Spring Data MongoDB dependency
  - `order(_id, orderId, orderDate, Product(productId, productName, unitPrice, quantity))` nesting structure.
  - The concepts are `@Document`, `@Id ObjectId objectId`, `@Field` Spring Data MongoDB annotations, and `CrudRepository<E, ID>` interface with `@Query` annotation using Json Structured queries (SQL works also) as a domain-specific language for querying from the database.
  - Relevant properties is `spring.data.mongodb.**`
- Neo4j as an example of graph database model through Spring Data Neo4j dependency
  - `order(orderId, orderDate)` and `product(productId, productName)` nodes with association `INCLUDES` from left to right between them having `unitPrice` and `quantity` attributes. 
  - The concepts are `@Node`, `@Id`, `@Relationship` and `@TargetNode` Spring Data Neo4j annotations and `CrudRepository<E, ID>` interface with `@Query` annotation using Cypher as a domain-specific language for querying from the database.
  - Relevant properties are `spring.data.neo4j.**` and `spring.neo4j.**`

### Rating ⭐⭐⭐⭐☆
- ✅ Implementation of the same conceptual data representation in various database models, sorcery that programmed code on the fly worked always at the first try 
- ⛔ Missing introduction of at least basic examples of use-cases for what each data model is suitable or not, more detailed comparison aside from implementation is missing

_____

## [Spring Data JDBC: Beyond the Obvious](https://springone.io/2021/sessions/spring-data-jdbc-beyond-the-obvious)
> "Strong Aggregates as a main concept of Spring Data JDBC: Whatever is reachable from the root of you aggregates is part of that aggregates and gets persisetd/loaded with that root"
- Length 52:39, watched on 2021-09-09, **#spring #data #jdbc**
- Jens Schauder as Staff Engineer, VMware
- Track: Intermediate/Advanced Spring

### Keynotes
- Spring Data offers a common abstraction for various kind of persitent stores, by abstraction is means that things look similar and it' by no means that it's possble to just swap just one database out and another one in, otherwise the common set of features would be limited and the undelying technology features are no blocked - things looks similar so working with one gives an easy way in the other. Sprnig Data is famous for the ability to define repositories as interfaces conceptually from the domain-driven design.
- Spring Data JPA is far more popular than Spring Data JDBC but it brings a problem that is very complex, ex. it tries to map a graph of objects/classes to graph of tables with no boundaries (lazy vs. eager) and it is needed to know what is behind saving and what is actually saving and what is controlled with cascade annotations.
- Spring Data JDBC is yet another support for relation databases, such as Spring Data JPA but without JPA, the key of its simplicity are strong aggregates, whatever is reachable from the root of you aggregates is part of that aggregates and gets persisetd/loaded with that root just as it is kind of prescribed by domain-driven design the concept of aggregates cmoes from.
- **User Defined IDS**
  - If we call `CrudRepository#ave` on entity, set its `@Id` to particular value that is not present in the database, it fails since `UPDATE` is executed isntead of `INSERT` (because `@Id` is filled) and results in 0 updated rows.
  - Solution is autowiring and calling `JdbcAggregateTepmlate#insert` that is used under the hood. Another solution is defining a bean `BeforeSaveCalback<Minion>` that generates for example `UUID` ID for the entity if it has not set ID yet.
- **JSON / Custom Conversinos**
   - We can persist an entity with an object property having further properties as JSON.
   - To write, implement `Converter<MyEntityData, JdbcValue>`, annotate converter with `@WritingConverter` and store as `JdbcValue.of(json, JDBCType.VARCHAR)`/
   - To read implement `Converter<JdbcValue, MyEntityData>`, annotate converter with `@ReadingConverter` and read from JSON
   - It is needed to cerate a configuration class (annotated with `@Configuration`) extending from AbstractJdbcConfiguration` overriding and registering a bean of `JdbcCustomConversions`.
 - **Bidirectional Relationships** 
   - In the relationship 1:N `Minon` has `Set<Toy>`, the full-args constructor is annotated with `@PersistenceConstructor` to mark it for Spring Data and set reference for each `Toy#setMinion` to `this`, and that reference in `Toy` must be `@Transient`.
   - Alternatively it is possible to use `AggregateReference<Minion, Long>` in `Toy` and use `@Query` in the `CrudRepository<Toy>` to get `Collection<Toy> by `Minion#getId()` from its `AggregateReference`.
 - **Caching**
   - Just use Spring Data caching mechanism enabled by `@EnableCaching` and placed `@Cacheable` annotatinos.
 - **Eager Loading References**
   - To load data in a single statement it is possible to use a view such as `ToyView extends Toy` to simply include all `Toy` fields and embedded `Minion` field using `@Embedded(onEmpt = Embedded.OnEmpty.USE_EMPTY, prefix = "minion_")` annotation and fetch them in a repository using `@Query` with a `JOIN statement`.

### Rating ⭐⭐⭐⭐⭐
- ✅ Very informative session about not-to-known Spring Data JDBC, easy to understand examples
- ⛔ -

_____

## [Microservices Testing at Scale](https://springone.io/2021/sessions/microservices-testing-at-scale)
> "Contract testing allows API producers and consumers work in a decoupled fashion"
- Length 22:58, watched on 2021-09-09, **#microservice #test**
- Kishore Kotaas as Sr Architect, Discover Financial Services
- Sindhu Nair as Principal Value Stream Architect, Discover Financial Services
 - Track: Architecture

### Keynotes
- Testing monolithic architecture heavy relies on End-To-End testing and prolonges testing cycle
- Testing microservice architecture involves testing a lot of small moving pieces but system integration becomes more complex 
- Unit testing (isolation, mocking and stubbing) ->  Contract testing (contract creation and verification) -> System integration testing (system entry points) -> Backwards compatibility testing (two-step process) -> Performance testing (virtualize dependencies, short intervals and quick feedback) -> Vulnerability testing -> -> Disruptive testing (dependency and API outage) -> E2E testing -> Browser compatibility testing (Selenium) -> Production Smoke testing (certificates, network connection)
- For disruptive testing is possible to use [Spring Boot Chaos Monkey](https://github.com/codecentric/chaos-monkey-spring-boot)

### Rating ⭐⭐⭐☆☆
- ✅ Interesting overview of the extended testing pyramid
- ⛔ Too much teoretical and abstract, missing real-live examples of what exactly is tested in each part

_____

## [A Spring Data’s Guide to Persistence](https://springone.io/2021/sessions/spring-datas-guide-to-persistence)
> "Spring Data is a familiar and consistent programming model that respects store specific traits"
- Length 53:54, watched on 2021-09-10, **#spring #data**
- Christoph Strobl as Spring Data Engineer, VMware
- Track: Beginner-Friendly Spring

### Keynotes
- Spring Data is not a silver bullet (doesn't manage indices), is not a magical tool, is not one API to rule them all.
- Spring Data module anatomy starts with Repository Interface with a default implementation.
  - In the case of JPA uses Entity Manger.
  - In the case of NoSQL stores and modules is sits upon a Template API that takes care of all the resource and transaction management.
    - It uses the *Mapping* layer responsible for converting domain entities to something that can be stored via the driver.
    - For some specific properties (for example `enum`) that the driver themselves are not understood by, there is a Conversion engine for type translation.
  - All of the above sits on top of the database driver and does all the heavy lifting.
- `Repository` ->` CrudRepository` (`findAll` /` findById` / `count` /` save` / `delete` / ...)>` PagingAndSortingRepository` (`findAll (Page / Sort)`)
  - Derived Fetch Queries, some data sources might need a little help with `@ Modifying` annotation for` UPDATE` / `DELETE` (might return` void` / `long` /` List <E> `for none, count or modifyied entities respectively.
    - `List <E> findXXX`: It fetches all matched entities which put a lot of pressure on the memory and runtime, alternatives are below.
    - `Page <E> getXXX`: Pages has set a chunk of data giving a defined rate range of matching entities and count, however, it needs to allocate resources every time the method is invoked.
    - `Slice <T> queryXXX`: WOrks like Pagination, but it doesn't know the total number of available pages (overhead of extra query) and only knows whether the next slice is available or not.
    - `Stream <E> searchXXX / streamXXX`: Streaming is the alternatives for continuous scrolling, however, calling` limit` or `skip` on Stream contradicts its benefits and it is needed to close the Stream properly to release the boundary sources and free memory.
    - `Flux <E> findXXX` is an alternative for the reactive world.
 - For read-operation, it is possible to use DTO Projection, Closed Interface Projection (interface with getters), or Open Interface Projection (interface with getters annotated with `@Value (" {# target ...} ")`.
 - Query By Example (`List <E> findAll (Example <E> probe)`) is a good fit for web from search binding.
 - Spring Data JPA has auditing support through `@ CreatedDate` and` @ LastModifiedDate` annotations and even adds who created/modified the entity if the information is provided through the implementation of Auditor and Spring Security has already implemented for it so it's only needed to plug it in and activate auditing.
  - Spring Data MongoDB has `@DBRef List <Employee>` and `@DocumentReference Manager` which is a native storage format for references instead of whole documents, analogically the Spring Data JPA uses` @Embedded Manager` (possibly is needed to use `@ AttributeOverrides ({}) `to avoid field names clashes) to flatten the mapped entity.
  - Spring Data JPA provides access to Stord Procedures, which is a piece of functionality stored in the database, through `@Procedure (" Employee.increaseSalary ")` fr the JPA-stored procedure having both input and output parameters.
  - Spring Data MongoDB has support for geospatial queries returning a result list including the distance from the target location and the average distance from all the found documents to the target location, ex. `GeoResults <E> findByOfficeLocationNear (Point p, Distance max)`.
  - There is always support for native queries if a derived method is not enough, such as `@ Query` for Spring Data JPA or` @ Aggregation` for Spring Data MongoDB.
  - Spring Data offers to add store-specific custom implementation using Fragment interfaces on top of `* Repository` interfaces, ie to provide implementation and extend within the repository interface that is looked for at the application start-up.
 - To tune performance, Spring Data offer * Repository Metrics *, * Logiles *, * Network Stats *, and * Query Planners *.

### Rating ⭐⭐⭐⭐⭐
- ✅ Comprehenisle dive into the anatomy of Spring Data module and relational and document data storages
- ⛔ The very same deep comparison of a graph database model (Neoj4) would be great, troubleshooting part was too way brief, nothing about named queries as promised

_____

## [Live Coding Spring Data Queries to the End of the Persistence Universe](https://springone.io/2021/sessions/introduction-to-spring-data)
> "The queries must flow"
- Length 55:32, watched on 2021-09-11, **#spring #data**
- Greg Turnquist as Principal Software Engineer, VMware
- Track: Beginner-Friendly Spring

### Keynotes
- Spring Data JPA has pre-baked `JpaRepositoy` that extends `PagingAndSotringReporitory` from Spring Data.
- For debugging, enable `spring.jpa.show-sql=true` and `logging.leel.org.springframework.data=TRACE`.
- Having 1:N relationship between Manager and Employee `entities` using Spring Data JPA:
  - `List<Employee> findByNameContainingIgnoreCase(String partialName)` for full-text search.
  - `List<Employee> findByManagerName(String managerName)` query navigates across relationships. 
- Use `@EnableJpaAuditin` and register `@EntityListeners(AuditingEntityListener.class)` on the `Employee` object to enable auditing through `@CreatedDate` and `@LastModifiedDate`.

### Rating ⭐⭐⭐☆☆
- ✅ Auditing introduction, very beginner-friendly
- ⛔ Since beginner-friendly the database structure could be introduced (especially how auditing stores additional data)

_____

## [Leap Ahead with Redis 6.2](https://springone.io/2021/sessions/leap-ahead-with-redis-62)
> "The 'Most Loved' database in StackOverflow's Developer survey for the 5th year in a row"
- Length 26:11, watched on 2021-09-11, **#spring #data #redis**
- Brian Sam-Bodden as Developer Advocate, Redis Labs
- DaShaun Carter as Partner Solution Architect, Redis
- Track: Beginner-Friendly Spring

### Keynotes
- Redis (162 clients in 50 languages) stores data in memory, not on disk, which brings <1ms latency
- Srping Data is a damily of project giving a Java/Spring idiomatic ways to access data from low-level constructs to higl-level OO abstractions in either non/reactive or functional way
- Spring Data Redis provides reasy configuration and access to Redis through low-level connectivity via Lettuce & Jedis libraries, provides `RedisTemplate` as a high-level abstraction for Redis operations (Ops) and implements key-value mappings and repositories.
- String: ValueOperations can be performed through `StringRedisTemplate#opsForValue` and maximum size of a Redis Key is 512MB and Redis value is 512MB
   - `redis-cli set stringKey stringValue` (`SET`) sets a key-value.
   - `redis-cli get stringKey` (`GET`) gets a value by key.
   - `redis-cli getset stringKey stringUpdatedValue` (`GETSET`) gets a value by key and and sets the value immediatelly in one operation.
   - `redis-cli getdel stringKey` (`GETDEL`) gets a value by key and deletes the key immediatelly.
   - `redis-cli getex stringKey ex 3` (`GETEX`) gets and expires a key in a certain number of seconds.
   - `redis-cli set stringKey stringValue exat 1662163200` (`PXAT`) sets and expires a key at the sprcifiec Unix time in seconds.
   - `redis-cli set stringKey stringValue pxat 1662163200000` (`PXAT`) sets and expires a key at the sprcifiec Unix time in milliseconds.
   - `redis-cli ttl stringKey` (`TTL`) returns the remaining time to live of a key that has a timeout.
 - Hash: HashOperations (`HSET`/`HMSET`/`HGETALL`)  can be performed through `StringRedisTemplate#opsForHash`, the hash maps identified by *keys* between string *fields* and string *values* closely resembles Java Map and can store over 4 billion field-value pairs.
   - `redis-cli hset hashKey currentTime "${date}"` (`HMET`) sets field in the hash stored at key to value.
   - `redis-cli hmset hashKey status "Good" name "Redis" greeting "Hi"` (`HSMET`) sets multiple fields in the hash but is deprecated as of Redis 4.0.0 in favor to `HSET`
   - `redis-cli hget hashKey greeting`  (`HGET`) returns the `value` associated with `field` in the hash stored at key.
   - `redis-cli hgetall hashKey`  (`HGETALL`) returns all fields and values of the hash stored at key.
   - `redis-cli hrandfield hashKey 4 WITHVALUES` (`HRANDFIELD`) returns array of random distinct fields (if positive count) or random fields with possible duplicates (if negative count). 
 - List: ListOperations can be performed through `ListOperations<K, V>` and they are implemented in Redis as a linked list but has enough commands to turn it into a stack, queue or any linear storage and store over 4 billion entries.
   - Adding: Pushing in `LPUSH`/`LPUSHX`/`RPUSH`/`RPUSHX`, inserting before/after `LINSERT` and setting the value at an index `LSET`.
   - Removing: Popping off `LPOP`/`RPOP`/`BLPOP`/`BRPOP` (including blocking operations), by value `LREM` and by index range `LTRIM`.
   - Accessing: By index `LINDEX` and by range `LRANGE`.
   - Between sits: Last from one/to firt in another `RPOPLPUSH`/`BRPOPLPUSH` and pop and then push `LMOVE`/`BLMOVE` (including blocking operations).
 - Set: SetOperations can be performed through `SetOperations<K, V>` and thery are collection of unique and unsorted string elements supported by operations such as union, intersection and subtraction, most operations perform in constant time (`O(n)`).
   - Use cases: unique item management, tracking OPs, content filtering.
   - Adding `SADD` and removing `SPOP`/`SREM`.
   - Accessing `SMEMBERS`/`SRANDMEMBERS and retrieving `SSCAN`.
   - Set info `SCARD`/`SISMEMBER`/`SMISMEMBER` and set operations `SDIF*`/`SINTER*`/`SUNION*`/`SMOVE`.
 - Sorted Set operations can be performed through `ZSetOperations<K, V>`, they are weighted sets, tuples with a *value* and a *score* and elements are always taken by their score or in ranges, in spring Data Redis uses `Set<TypedTuple<E>>` data type.
   - Use cases: Prioriy queues, low-latency leaderboards or secondary indexing in general 
   - `redis-cli zadd game1 100 "Frank" 740 "Jennifer" 200 "Pieter" 512 "Dave" 690 "Ana"` (`ZADD`)
   - `redis-cli zrange game1 0 -1 wihscores` (`ZRANGE`)
   - `redis-cli zinter 2 game1 game2 wihscores` / `redis-cli zinter 2 game1 game2 withscores aggregate max` (`ZINTER`) 
   - `redis-cli zdiff 2 game1 game2 withscores`
   - `redis-cli zadd game1 100 "Foo"` (`ZADD`)
 - Geo: GeoOperations can be performed through `StringRedisTemplate#opsForGeo`, it is a sorted set as a latitude and longitude encoded into the score of thesorted set using the geohash algorithm.
   - Sicne it is still a sorted set, it is possible to use `Z*` commands 
   - `redis-cli GEOAD running-poi -94.238226 39.029377 "Lake"
   - `redis-cli GEODIST running-poi "Lake" "Park"
 - Streams before Redis 6.2 could be only trimmed to an exact or aproximate number of entries which were odd as it defies stream processing
   - The rule of thumb is that each entry in a stream must have a unique ID greater than any previously seen in the stream (Redis by  defaut uses millisecods timestamps for this) and now allows you to trim based on ID.
 - Redis team is up to extending and complementing Spring Data Redis with:
  - Access to module commands via Spring's Tepmlates, multi-model obect-mapping support, JSON obect-mapping and RediSearch integration, Redis Graph oriented-mapping, RediSearch integration for existing Redis Hash mapped entities. 
- Redis Modules Tepmlates follow Spring Data Redis `opsForXXX()` pattern and provide Native way to interact at the command-level with RedisSON, RedisGraph, RediSearch, RedisAI, RedisBloom, and RedisTimeSeries

### Rating ⭐⭐⭐⭐⭐
- ✅ Enthustiatic talk covering wide-range of Redis topics with practical examples with some ease
- ⛔ Some commands could be omitted in favor of where Redis aim now as said at the end of the session

_____

## [Winning the Lottery with Spring: A Microservices Case Study for the Dutch Lotteries](https://springone.io/2021/sessions/winning-the-lottery-with-spring)

> "Microservices architecture built using state-of-the-art Spring Boot and Cloud components"
- Length 27:12, watched on 2021-09-12, **#spring #microservices**
- Joris Kuipers as CTO, Trifork
- Track: Architecture

### Keynotes
- Case study of the integration platform developed for the Dutch Lotteries
- Architecture: Separate domains (verticals - specific games, subscriptions, players...) and service types (horizontals)
- Project Setup: Every service is Spring Boot or Cloud app running on AWS EKS as AWS proprietary Docker orchestrator (K8S) using blocking HTTP for inter-service communication (started at the end of 2017, but too early for reactive programming as Spring was starting too, even though it would have been a good fit since asynchronous non-blocking is basically the bread and butter of building gateways and integrated solutions).
- Currently around 30 services ad a bunch of libraries inside of a single GIT repository with a single Gradle build that produces all of the actual Docker images because it is easy to build shared libraries used by a variety of services so no artifactory is needed. 
  - `libs` module are only Java libraries (not Dockerized servicies): `accoung-status-store-client`, `auto-parameter-store-config`, `common-error-handling`, `common-potcodeservice-client`, `encryption`, `experience-web-shared`, `gateway-logging`, `gateway-monitoring`, `gateway-specification`, `gateway-testing`, `gateway-utils`, `http-client-autoconfiguer`, `open-api-specifications`, `sqs`, etc...
  - `inlane`, `marketing`, `players` (sample submodules: `player-experience`, `player-experience-spec`, `player-igaming`, `player-process`, `player-specs`, `player-system`, `player-system-client`, etc...)
- **Autoconfiguration for the people**
  - Spring Boot autoconfiguration is the main and most visible feature used extensively within the framework but not restricted to Spring Boot itself.
  - Although it seems like a black-box or magic it is nothing more than conditional configuration classes providing beans that may or may not be initiated at startup based on certain conditions (classpath presence, something defined...), automatically applied and listed in `META-INF/spring.factories`.
  - Custom autoconfiguration benefits in encapsulation and dynamic configuration (conditions, overridable defaults) and making components auto-configurable with default properties enable configuration options discovery (`@ConfigurationProperties` allows IDE auto-completion).
  - Key concepts: `@Configuration`, `@PropertySource(value="classpath:httpclientlogging.properties")`, `@Import(HttpConnectionPoolHealthIndicaor.class)`, `@ConfigurationProperties("http.client"` on the properties POJO class, and `@Bean` definitions including `@Primary`, `@ConfitionalOnMissingBean` and `@Order`.
  - Examples: Custom JSON marshaling configuration, error handling (involves JSON response parsing), authentication (OAuth bearer token, basic auth), etc...
- **Observability for messaging**
  - Distributed Tracking is allowed by Spring Sleuth that propagates correlation ID per logical request called Trace ID and is instrumented by many Spring components out of the box.
  - Spring Cloud AWS for SQS integration (point-to-point solution - templates for sending, listener container for receiving) + Sleuth integration for message headers = To correlate asynchronous logging as a port of regular flow and provide Admin tool to link error logs for dead-lettered messages
- **Spring Cloud Netflix**
  - Part of the start of Spring Cloud allowed Netflix OSS stack to be used with Spring Boot (Eureka, Zuul, Ribbon, Hystrix...), but Netflix has stopped maintenance, and Spring support announced to stop as well providing alternatives.
  - `Experience API` -> `Process API` -> `System API` - sometimes the Process API needed to do actual work and sometimes, however, just proxy through so they wanted to have an automatic way of doing that proxy which is what Zuul did
  - With replacing deprecating Zuul they were forced to call `Experience API` -> `System API` directly in some cases, but they needed something to proxy 3rd party libraries, so they used Spring Cloud Gateway MVC (not SPring Cloud Gateway) which is a simple `RestTemplate` wrapper (`ProxyExchange passed to controller method allows for adding headers & query params, changing path and making the actual request) with Spring MVC integration for building proxies supporting reactive as well.

### Rating ⭐⭐⭐⭐⭐
- ✅ Great use-case talk especially about technology and know-how of using custom Spring Boot autoconfiguration and replacing Spring Netflix
- ⛔ Lack of time for more detailed API gateway description and circuit breaker solution

_____

## [Live Coding Spring, Kafka, & Elasticsearch: Personalized Search Results on Ranking and User Profile](https://springone.io/2021/sessions/spring-kafka-elasticsearch)
- Length 26:42, watched on 2021-09-13, **#spring #elasticsearch**
- Erdem Günay as CTO, Layermark
- Track: Architecture

### Keynotes
- ElasticSearch based indexed search using analyzers and filters with a boost by popularity and by user behavior.
- `GET /_cat/indices` returns all the indicies
- `POST /content/_search` queries the `content` index but an exception is thrown if index is not found (`PUT /content`/`POST /content/_bulk`).
- **ElasticSearch Analyzers**
  - By default, ElasticSearch finds by an exact match, to enable easy search using a single letter ignoring accented characters (`é`, `í`, etc...) it is needed to use ElasticSearch Analyzers utilizing `POST _analyze` with `"tokenizer": "standard"` and `"char_filter"` with `pattern_replace` "type` to replace anything that is not an alphanumeric character.
  - To get rid of capital letters and non-ASCII characters, it is needed to add token `"filter" : ["asciifolding", "lowercase"]` and specific `edge-ngram` among them.
  - It is needed to delete the former index and recreate the index.
  - Each `hit` has a `_score` that sets the element order in the returned structure.
  - For search by fields, it is possible to add *boosting*, ex. boost the search of artist name `artist_name` by a factor of 5 (exact match should have a bigger score) as `artist_name^5` or `artist_name.prefix^1` where are the generated tokens stored in. 
  - `"fuzziness" : 1` enables to match other elements (ex. `"query": "sezan"` would match `Selena Gomez` with a low `_score` since there is a partial match in individual letters from search (basically allows typos).
- **Boosting results by popularity**
  - If search is based on a single letter (`s`), `Shakira` might be places below `Selena Goméz` although the popularity sais otherwise (I liek Shakira more, though). It is needed to enable scoring on search through `POST /content/_search` and provide `"script_score"` in `"functions"` in `"function_score"` in `"query"`: `"script" { "source" : "Math.max(((!doc['ranking'].empty ) ? Math.log10(doc.['ranking'].value) : 1), 1)", "lang" : "painless" }`.
  - Assuming the popularity is updated programmatically (200 asynchronous hits by Kafka) it is needed to process the listen-event messages and place them in listen-event indices using `POST /listen-event-*/_search/`. User profiles are also getting generated (`POST /user-profile/_search`).
 - **Boosting by user behavior**
   - If a particular user searches for a certain element, that element should be bosted in the search for that particular user only. 
   - Another funciton must be taken into account similarly as previous boosting: `"script" : { "source" : "params.boosts.get(doc[params.artistIdFieldName].value)", "lang" : "painless", "params" : { .. } }`.

### Rating ⭐⭐⭐⭐☆
- ✅ Informative overview of what is ElasticSearch capable of, although, the live demo is impossible to follow but still impressive
- ⛔ The way result popularity in real-time was updated from Kafka was not really clearly explained, it's not clear why Kafka figures in the demo if an easier approach could be used and the title is misleading then, data structure could be shown as not everybody has experience with ElasticSearch (all because I guess mostly caused by of lack of time), I can't extract the gist or quote of the talk into the header

_____

## [Debugging Complex Issues in Web Applications](https://springone.io/2021/sessions/debugging-complex-issues-in-web-applications)
> "It is often required to simulate lost connection at some point by literally two machines and "pulling out the cable."
- Length 51:15, watched on 2021-09-14, **#spring #tomcat**
- Mark Thomas as Staff Engineer, VMware
- Track: Intermediate/Advanced Spring

### Keynotes
- **Complex issues** are subjective (everybody has a different understanding o this term), and there are three factors that are not completely independent but it tends one dominates more than the other.
  - Issue that isn't 100% repeatable which typically means harder to debug, it drags the process out (get data, analyze, fix, repeat).
  - Only occurs under load, which generates an awful load of application/debug logs, Wireshark, and network traces.
  - Issues around concurrency tend to happen when there are multiple threads interacting and a problem only occurs when a particular sequence of events happens between those threads.
  - Methodology: Identify at a high level, record state before/after and check the consistency of them with expectations, sometimes it is needed to record multiple points.
    - To defy the statistical variation, it is needed more samples, load, and tests: at least 20 tests, at least 5 passes, at least 5 failures, and keep adding tests and load until you meet all three.
    - Beware and the issue can have multiple root causes.
- **Use-case: [Large and concurrent HTTP/2 responses](https://tomcat.markmail.org/thread/texcre345tmyn337)** - well-described, 1-2 days to fix
  - Trouble with HTTP/2 (HTTP/2 connections are multiplexed: Multiple streams are trying to write and semaphore ensures only one writes at a time) during bulk data transfer (server -> client), multiple streams on same connection blocked indefinitely (configured an infinite timeout, so blocked until connection timeout).
    - > When a write operation is stuck servlet is not able to push any data to the client and the client is also stuck waiting for more data. There wasn't any error/exception at the client/server. `streamReadTimeout` and `streamWriteTimeout` are configured as `-1` so they are infinitely waiting for the write semaphore.
    - Described details for a test case to be coded: writing large files (1GB - 5GB) on three or more concurrent streams.
    - Described working HTTP/1.1 and non-working configurations (HTTP/2), reproducible both on blocking and non-blocking API
  - Identify root cause process:
    1. Since fairly reproducible, it was possible to continually exclude functionality to narrow the focus: Disabling asyncIO proved it is where to start looking and provided a user a workaround (disable this functionality).
    2. It was possible to see threads waiting for semaphore (it should be released by Poller indicating ready to write), code review started (possible root cause was non-volatile `interestOps` flag) but volatile `interestOps` on a higher level of tests didn't show the issue was fixed as the test was failing - the importance of sufficient testing sample.
    3. Next step was to debug Socket/Poller interactions but added logging changed time timing and issue became less repeatable so the logging strategy was needed to be changed: copy relevant information to variables and log them after failure or event of interest that much less likely affects timing - but after a log of debugging Poller was working correctly.
    4. Poller was signaling write was possible but `OperationState` was `null` which was potential root cause because the event couldn't be processed and semaphore was never released - although it was fixed, since reading and write operations are similar, the same error could exist elsewhere (read also affected but nobody haven't stumbled across it yet).
    5. Fix: https://github.com/apache/tomcat/commit/92b91857
- **Use-case: [Connection drops before writing response](https://tomcat.markmail.org/thread/bf6oz7ibxccvodd2)** ~ well-written report but, the presenter had no access to the system where the issue could be created, 6 weeks to fix
  - Very occasionally Tomcat didn't send a response shown in the access log, no exceptions and Wireshark shows the GET request was followed by a TCP FIN packet from Tomcat (clean TCP close).
  - Identify root cause process:
    1. Asked various questions to try to eliminating features and/or possible failures: small response ~1kB (small enough to buffer entirely), typical response time 60m (not timeout-related), FIN sent 100µs after request received (no timeout-related), the request was fully sent (no waiting for the rest of the request and not malformed), User-agent -> Firewall -> Nginx -> Tomcat, HTTP/1.0 request (ruled out HTTP/2), no indicator from network traces from Tomcat and Nginx, unique request IDS aided correlation across logs, issue started in the last month but no obvious changes released, systems were lightly loaded (20 requests/s).
    2. Configuration changes: Switching from BIO to NIO didn't fix the issue (not in endpoint specific code, less likely JVM issue),  added `%b` configuration to access log to suggest JSP is generating response (it was), no GZIP (no compression involved), no obvious explanation.
    3. Custom debug code to provide detail on when things were happening (who is closing the socket) because it was closed long before Tomcat tried to write, but neither Tomcat nor the application was closing it - what the hell was it?
    4. After more logging, it showed the exception "Bad file descriptor" was swallowed, because it was assumed to be a dropped client connection (Tomcat changed to debug-log them), no indication file descriptors ran out, no other connections present between Nginx and Tomcat when the issue occurred and no indication of JRE mishandled file descriptors.
    5. `strace` time showed the socket close came from somewhere in the JRE and an attempt to correlate with thread dumps to identify where the close occurred showed a native library incorrectly managed the file descriptors associated with a fork and closed a file descriptor twice - in same cases the descriptor has already been re-used for the network connection which was hence closed..
    6. Vendor accepted the native library (PDFTron) was at fault and provided instructions to disable the use, but Tomcat recommended switching to HTTP/1.1 for the Nginx/Tomcat connection to assure fewer and persistent new connections do not constantly change the file descriptor so the native library was less likely is going to have the same one and then close it on you.
- **Use-case: [Response write does not compile](https://github.com/spring-projects/spring-framework/issues/26434)** ~ originate on Spring Framework's issue tracker, well-written, 6 weeks to fix
  - Small number of response writing fails to complete with WebFlux on Tomcat under load, low repeatability was the biggest issue as it was timing-sensitive.
  - Multiple issues identified: Spring handling of failed flushes, incorrect Tomcat error handling (attempted to flush the error page content after an I/O write error overwritten the original one, IO errs were not triggering to the error listener, Tomcat assumed `IOEception` would be seen bu the container but WebFlux swallowed them).
  - After fixing the Spring issue, Tomcat now calls error listener before internal error handling and it ended with [JDK bug](https://bugs.openjdk.java.net/browse/JDK-8263243) and [Ubuntu bug](https://bugs.launchpad.net/ubuntu/+source/linux/+bug/1924298) because for once incoming connection there were two firings of the socket accept method and there should absolutely be a one-to-one mapping (so there were two threads processing the same socket).
- **Techniques**
  - Logging and Wireshark should use a 5-minute rolling window, don't be afraid to use `ERROR` logs, the network latency-related issues can be simulated in the supervisor, choose the load generator carefully as they are not always completely spec-compliant and might behave not the way you think (especially HTTP/2), it is often required to simulate lost connection at some point by literally two machines and "pulling out the cable", test on multiple platforms since VM or bare metal seems to be less of an issue.

### Rating ⭐⭐⭐⭐☆
- ✅ Impressive walkthrough of debugging truly complex issues around Tomcat including network communication or Ubuntu, great explanation of the steps proceeded.
- ⛔ All issues were well-written and an example of a poor one would be nice, the lip-smacking was very intensive and annoying with all due respect to the speaker.

_____

## [Spring Boot—Production Boost](https://springone.io/2021/sessions/spring-boot-production-boost)
> ""
- Length 26:09, watched on 2021-09-14, **#spring #kubernetes**
- Thomas Vitale as Senior Software Engineer, Systematic
- Track: Beginner-Friendly Spring

...

_____

## [How to Use KPIs in an Agile Delivery Environment](https://springone.io/2021/sessions/how-to-use-kpis-in-an-agile-delivery-environment)
> ""
- Length 24:15, watched on 2021-09-14, **#agile #project #management #kpi**
- Arijit Sarbagna as Director - Agile & DevSecOps, Atos
- Track: Agile Leadership

...

_____

## [Why Every Software Team Should Have a Designer](https://springone.io/2021/sessions/why-every-software-team-should-have-a-designer)
> ""
- Length 24:15, watched on 2021-09-16, **#agile #project #management**
- Antonia Horvath as Delivery Lead & Design Manager, VMware Tanzu Labs
- Track: Agile Leadership

...
