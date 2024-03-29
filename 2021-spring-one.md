# [Spring One 2021](https://springone.io/2021)

|                         |                | Remark                                                                              |
|-------------------------|----------------|-------------------------------------------------------------------------------------|
| Location                | 🌎 Worldwide   |                                                                                     |
| Date                    | September 2021 |                                                                                     |
| Languages               | English 🇺🇸     |                                                                                     |
| Paid                    | No             |                                                                                     |
| Conference availability | Online         |                                                                                     |
| Records availability    | Yes, unlimited | https://springone.io/2021/schedule#day1 and https://springone.io/2021/schedule#day2 |

## Attended sessions list

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
| [How to Start Your Application Modernization Journey](#how-to-start-your-application-modernization-journey) | #agile #organization #learning #microservices | 25:43 | Agile Leadership |
| [Staying Ahead of the Curve](#staying-ahead-of-the-curve)                                         | #agile #organization #learning #microservices | 54:20 | Beginner-Friendly Spring |
| [A Tour of the Modern Java Platform](#a-tour-of-the-modern-java-platform)                         | #java #spring #docker #containers #graalvm | 57:11 | Architecture |
| [The Art of Clean Code](#the-art-of-clean-code)                                                   | #java                         | 14:27 | Track: Architecture           |
| [Bootiful Vaccine Scavenger: A Tale of the Pragmatic Spring Framework](#bootiful-vaccine-scavenger-a-tale-of-the-pragmatic-spring-framework) | #spring #spring-boot #spring-cloud spring-cloud-streams #rabbitmq | 25:30 | Track: Beginner-Friendly Spring |
| [How Spring Cloud Gateway Orchestrated Our App Modernization](#how-spring-cloud-gateway-orchestrated-our-app-modernization) | #spring #spring-cloud #devops | 25:16 | Architecture |

_____

## [How To Be a Java Automated Testing Superstar](https://springone.io/2021/sessions/how-to-be-a-java-automated-testing-superstar)
> "Write automated tests until they give me the confidence to deploy PROD without manual intervention."
- Length 26:24, watched on 2021-09-07, **#architecture #test**
- Billy Korando as Java Developer Advocate, Oracle
- Track: Architecture
- Language: English 🇺🇸

### Keynotes
- Automated tests should be human-readable and treated as same as the production code. They are repeatable and auditable.
- **Dependency iceberg** says that our code is just a tip of all the code the application runs on. The dependencies are below.
  - Most of the code are dependencies, feature and performance enhancements (Spring libraries, JSON/XML mappers, ORM implementation, servlets, etc.), and security patches.
  - We cannot rely 100% on it, especially if we use the last stable versions. On the other hand, old versions have security flaws (Struts).
- How many automated tests should I write? Whatever gives me the confidence to deploy PROD without manual intervention (i.e. code coverage is just informative).
- Manual testing is still needed but it is exploratory testing.

### Impression ⭐⭐⭐⭐☆
- ✅ Theoretical aspects and importance of testing, best practices of unit testing.
- ⛔ Too short (not the speaker's fault), code examples weren't that impressive, no mention of [BDD](https://en.wikipedia.org/wiki/Behavior-driven_development) approach.

_____

## [Deploy Code into Production Faster on Kubernetes](https://springone.io/2021/sessions/modern-application-configuration-in-kubernetes)
> "Developer experience on DIY platforms is lacking."
- Length 27:31, watched on 2021-09-07, **#devops #cloud #native #microservices**
- Valentina Alaria as Director Product Management, VMware
- Track: Cloud Native Platforms
- Language: English 🇺🇸

### Keynotes
- Most of the Kubernetes offerings are delivered as a bag of parts:
  - 63 % of organizations, that use K8S, use it as internal platforms or build internal platforms.
  - 94 % of organizations, if use K8S, building internal platforms use more than one platform.
  - 58 % of organizations agree that architectural decision-making has gotten harder.
- Developer experience on DIY platforms is lacking. Developers must still maintain containers, configure containers that run through multiple layers of YAML, and manage IT and security aspects.
- Importance lies in tooling to help developers: leverage automatized DevOps practices, enforce organizational best practices, app-aware platform, and preconfigured templates by Ops.

### Impression ⭐⭐☆☆☆
- ✅ Beginner-friendly introduction, on-spot developer concerns identification.
- ⛔ The structure doesn't match the agenda in the introduction and is a bit chaotic, rather Tanzu platform promotion, lacks expected pure K8S tips

_____

## [Modern Application Configuration in Kubernetes](https://springone.io/2021/sessions/modern-application-configuration-in-kubernetes)
> "Spring Cloud Config vs. K8S Config-maps and secrets."
- Length 26:49, watched on 2021-09-07, **#devops #kubernetes #spring #cloud**
- Craig Walls as Engineer, VMware
- Track: Architecture
- Language: English 🇺🇸

### Keynotes
- Spring applications environment configuration is based on Spring Environment Abstraction as of Spring 3.1 (`application.properties`, `application.yml`, command-args, JVM system properties...).
- They can be in the filesystem and are very difficult to audit and manage across multiple applications and instances.
  - Spring Environment Abstraction is extensible and has a solution for versioned (Git, Vault, DB, CredHub...), audited (git log) and centralized configuration - Spring Cloud Config Server
  - Such configuration must be read from the server and merged into Environment - Spring Cloud Config Server client library
  - Although Spring Config Server/Client can run on K8S, it must be merged into Resources, that are K8S native, like config-maps and secrets - Tenzu
- **Spring Cloud Config:** Central management of properties, can be versioned, can be audited, HTTP-based property consumption, probably should be secured, requires client-size library or code
- **K8S Config-maps and secrets:** Doesn't require special client code, K8S-native, not centrally managed, versioning/auditing is not built-in, can leverage K8S-native security

### Impression ⭐⭐⭐⭐⭐
- ✅ Very catchy speech, an excellent introduction to the environment properties management problem and comparison of approaches
- ⛔ The speaker has only one session

_____

## [You Can Be Cloud Native, Too](https://springone.io/2021/sessions/you-can-be-cloud-native-too)
- Length 27:00, watched on 2021-09-07, **#cloud #native**
- Hananiel Sarella as Software Engineer, VMware
- Track: Beginner-Friendly Spring
- Language: English 🇺🇸

### Keynotes
- Pros: Microservice architecture provides easy-to-maintain, test, and deploy services, teams can be scaled, polyglot-friendly,
- Cons: Distribute systems are rather complex and interaction is difficult to test, memory consumption and overhead
- Cloud-native patterns: Consistent management, run everywhere, secure, seamlessly adopt new environments, distributed systems patterns and abstractions
- Steeltoe Project introduction on top of the .NET foundation enables building production-grade and cloud-native microsystems in a simplified way quickly to stand up
  - Scalability (service discovery, configuration providers), Resilience (circuit breaker, bulkhead, client-side load balancing), Ease of Use (initializer, autoconfiguration, platform providers, and connectors such as DB, MQ, OAuth), Observability (management endpoints, dynamic logging, distributed tracing, metrics), Security (SSO, JWT auth, certificates), Messaging (stream processing)

### Impression ⭐⭐⭐☆☆
- ✅ Broad overview of microservice architecture facilities and difficulties
- ⛔ Missing introduction into cloud-native concepts since this is marked as beginner-friendly, too many buzzwords, .NET examples

_____

## [A Developer’s Introduction to Containers](https://springone.io/2021/sessions/a-developers-introduction-to-containers)
> "Container is process isolation."
- Length 26:15, watched on 2021-09-08, **#containers #devops**
- Nigel Brown as Senior Open Source Community Manager, VMware
- Track: Cloud Native Platforms
- Language: English 🇺🇸

### Keynotes
- Container is a process or group of processes running in isolation, it is great for portability and security
- The way of achieving the process isolation is by leveraging several features of the Linux kernel:
- **[Namespaces](https://en.wikipedia.org/wiki/Linux_namespaces)**
  - They wrap global system resources in an abstraction that makes it appear to the process within the namespace, that they have their own instance of the resource.
  - Process *one* and *zero* are typically reserved for what it takes to initialize our OS. In a container, typically, the application is running an application with process id *one* That's a whole instance of the process id counter that's working inside of the container that is different from what's happening outside and that's achieved by having a separate namespace from within which to work.
- **[cgroups](https://en.wikipedia.org/wiki/Cgroups)**
  - Control groups allow processes to be organized into hierarchical groups whose usage of various types of resources can be then limited and monitored.
  - Basically, it allows assigning a maximum number of resources each group can allocate to ensure your critical system processes always have the resources they need to run.

### Impression ⭐⭐⭐⭐⭐
- ✅ Excellent explanation of the container and Linux kernel concepts, simple but nice workshop
- ⛔ Slides would be better to support the ideas at the beginning

_____

## [Building Fast and Scalable Persistence Layers with Spring Data JPA](https://springone.io/2021/sessions/fast-and-scalable-persistence-layers-with-spring-data-jpa)
> "Favour DTO interfaces projections without advanced techniques (SpEL, nested associations) for read-operations over managed entities."
- Length 54:50, watched on 2021-09-08, **#spring #jpa #hibernate**
- Thorben Janssen as a Freelancer, Self-employed
- Track: Intermediate/Advanced Spring
- Language: English 🇺🇸

### Keynotes
- Hibernate statistics: Properties `hibernate.generate_statistics=true`, `hibernate.session.events.log.LOG_QUERIES_SLOWER+THAN_MS=3` and logging `org.hibernate.stats=DEBUG` (for DEV purposes).
- **Association management**
- `FetchType` recommendation:
  - To-many relationships: Stick to the default mapping `FetchType.LAZY` and use fetching for specific queries if required.
    - To-one relationships: Check existing mappings individually and use `FetchType.LAZY` for new ones.
  - N+1 problem that lazy fetching introduces:
    - Fetch all required entities with one query using Fetch Joins (`JOIN FETCH` in `@Query` or Entity Graphs (@NamedEntityGraph` and `@EntityGraph`)
    - Beware of left-joining as the complexity of the queue raises and it becomes slower. Although it's recommended to not join more than one association, it also depends on whether it contains 3 or thousands of rows.
  - Hibernate and many-to-many:
    - Hibernate handles `List` inefficiently (it removes all associations and adds remaining ones) so is better to use `Set`.
- **Projections** help to fine-tune the data that you need, so less data is selected from the database
  - Write-operations:
    - Entities are managed by the current persistence context, which means at the end of the transaction the managed entity is updated in the database through queries
  - Read-operations: They don't need lifecycle management overhead (no `INSERT`/`UPDATE`/`DELETE`).
    - Scalar values are object arrays (`Obejct[]`) and need to remember the order in the `SELECT` clause.
    - DTO classes (without `@Entity` for pure JPA) and interfaces with matching getter methods (easier, Spring Data JPA generates a class based on the definition) are preferred over scalar values
- **Advanced DTO projections pitfalls**
  - Nested associations such as a getter returning `List<ClientDtoProjecion>` on an interface-based DTO projection defies all the benefits of the DTO projections introduced earlier
  - SpEL such as returning first and last name together using `@Value("#{target.lastName + ', ' + target.firstName}") over a getter that actually selects a whole entity and it is better to use a `default` interface method performing the concatenation instead and preserve the benefits of DTO projections
- **Caching**
- 1st level cache:
  - Each Hibernate session has 1st level cache assuring we have only one object representation of each record in the database within each session, but it is useless performance-wise when each user has their session.
- 2nd level cache:
  - It is a session-independent entity store containing entity objects and is used whenever an entity is found by its primary key (or if associations are traversed), but it creates some additional problems because now this external cache is needed to keep in sync (check first) that creates a small overhead and it's needed to compensate with a higher number of hits (rule of thumb is at least 9-10 reads per 1 write operation).
  - It needs to be activated in properties with a specific cache mode where `ENABLE_SELECTIVE` and `DISABLE_SELECTIVE` is recommended over `ALL`/`NONE`/`UNSPECIFIED` and managed through `@Cacheable` annotation on the repository class/method or entity class level.
  - Tip: Place `@Cache(use = CacheCocurrencyStrategy.TRANSACTIONAL)` over many-to-many associations and all associations on entities that don't map the foreign key column, because in these cases Hibernate doesn't cache the *association* between these two objects but *only* the objects themselves.

### Impression ⭐⭐⭐⭐⭐
- ✅ Practical workshop with an on-spot set of tips for working with Hibernate and Spring Data JPA effectively
- ⛔ An alternative to SpEL was introduced but not to the nested association within advanced DTO projection

_____

## [Packaging and Distributing Applications for Kubernetes](https://springone.io/2021/sessions/packaging-and-distributing-applications-for-kubernetes)
> "Carvel is a composable Kubernetes tool suite."
- Length 24:55, watched on 2021-09-08, **#devops #kubernetes**
- Ian Zink as Staff Software Engineer, VMware
- Nitasha Verma as Solutions Engineer, VMware
- Track: Architecture
- Language: English 🇺🇸

### Keynotes
- Relocating K8S configurations and containers in the hands of their customers as a secure, consistent, and unified distribution within the framework of their existing ecosystem is clumsy.
- Application lifecycle (packaging and deployment on K8S): Author Configuration -> Package and Distribution -> Customizing Configuration -> Deploy to Cluster.
- Carvel is a composable Kubernetes tool suite, which provides a set of reliable, single-purpose, composable tools that aid in your application building, configuration, and deployment to Kubernetes. Basic tools:
  - `ytt`: Template and overlay K8S via YAML structures.
  - `kbld`: Build or reference container images in K8S configuration in an immutable way.
  - `kapp`: Install, upgrade, and delete multiple K8S resources as one application.
  - `imgpkg`: Bundle and relocate application configuration (with images) via Docker registers.

### Impression ⭐⭐⭐☆☆
- ✅ Well-structured presentation with a demo, they were able to find a workaround for an unexpected error they faced during the demo
- ⛔ Overly abstract terms (configuration, bundle, registers...) and commands in the demo were insufficiently described

______

## [From Spring Framework 5.3 to 6.0](https://springone.io/2021/sessions/from-spring-framework-5-3-to-6-0)
> "Spring Framework **5.3.x** remains in active development and Spring Framework **6.0** will be the beginning of a new generation."
- Length 25:34, watched on 2021-09-08, **#java #spring #jakarta**
- Juergen Hoeller as Spring Framework Project Lead, VMware
- Track: Intermediate/Advanced Spring
- Language: English 🇺🇸

### Keynotes
- Spring Framework **5.3.x**:
  - Java 17 support against a Java 8 baseline, support in Spring Boot 2.6 as of November 2021.
  - Java EE 8 focus agasint a Java EE 7 baseline.
- Spring Framework **6.0**:
  - Development branch (main) will be established in mid of September, the milestone phase at the end of 2021 (`6.0.M1` version), release candidate phase in mid-2022 (`6.0.RC1`). and `6.0` GA in October 2022.
  - Release cadence is yet undecided, might follow Boot's half-year rhythm.
  - Spring Native initiative moves into Spring proper, AOT processed metadata for regular JVM deployment as well.
  - Introduces core abstractions
- Spring Boot 2.7 as of May 2022.
- Spring Boot 3.0 introduces a starter for native applications, build plugins and support for specific GraalVM versions, and auto-configuring the observability backend
- Java 17 enforces illegal access rules, and no general escape hatch anymore.

### Impression ⭐⭐⭐☆☆
- ✅ Interesting overview of upcoming versions and timing
- ⛔ Missing examples of existing problems that new features would resolve, 60% of the time is rather focused on terms than features

_____

## [Spring Security 5.5 From Taxi to Takeoff](https://springone.io/2021/sessions/spring-security-5-5)
> "Spring Security integrates the Spring Native for all of its authentication mechanisms and all of its authorization models."
- Length 51:05, watched on 2021-09-08, **#spring #security**
- Josh Cummings as Software Engineer, VMware
- Marcus Da Coregio as Software Engineer, VMware
- Steve Riesenberg as Software Engineer, VMware
- Track: Beginner-Friendly Spring
- Language: English 🇺🇸

### Keynotes
- **Secured by default first principle**
  - `spring-boot-starter-security` present on classpath means that every endpoint either user-generated or Spring Boot-generated (`GET /error`) requires Basic authentication with `user` username and randomly generated password printed into the console (protection if Spring profile is not changed by mistake).
  - The random password is generated until the default security configuration is overwritten (`UserDetailsService` bean).
- **Personalize the application to the logged user**
  - Thread local `SecurityContextHolder` gives access to the application available anywhere on the current thread-bound in a servlet application to the current request.
  - `SecurityContextHolder.getContext().getAuthentication()` gives some of that information about the currently logged-in user, but there are little difficulties with testing this code because it is needed to mock out the thread-local pattern, security context, and authentication, so method injection is preferred (`List<Flight> getFights(Authentication auth)`).
- **Authorization of a certain endpoint**
- Some endpoints must be restricted to certain users, so it is needed to define either *roles* or *authorities* to them in `UserDetailsService` bean and map endpoints to the authority through `SecurityFilterChain` bean (`.httpBasic(Customizer.withDefaults())` must be added though).
- It is needed to provide a CSRF token to pass through the `CsrfFilter` to prevent [cross-site request forgery](https://owasp.org/www-community/attacks/csrf), ex. `.csrf((csrf) -> csrf.csrfTokenRepository(CookieCsrfTokenRepository.withHttpOnlyFalse())` and defining `CorsConfigurationSource` bean - The preflight (`OPTIONS` HTTP method) request conains the CORS headers on response and in the request to `POST`/`PUT` is present header `Access-Control-Allow-*`, and `Cookie` with the `XSRF-TOKEN` token and `X-XSRF-TOKEN` header itself together called *double submitting cookie*.
- It is needed to manage CORS to allow call endpoints from the endpoint using `.cors(Customizer.withDefaults())`.
- **Insecure direct object reference vulnerability**
  - Secure wildcard endpoints such as `PUT /{flightId}/taxi` are vulnerable as it is not checked if the object to be modified is compliant with the current authentication.
  - It is not preferred to weave the authentication behavior into the business logic and use more declarative security patterns using the domain-specific language (DSL), ex. `@PostAuthorizate("returnObject?.pilotId == authentication.name")` for outputs or `@PreAuthorize` for inputs are both compliant with the Spring transaction management and upon exception thrown by this construct any kind of change to the database will be rolled back - to get Spring Security to honor these annotations, `@EnableGlobalMethodSecurity(prePostEnabled = true)` is required.
- **Externalize the authorization** creating a `@Component` implementing `AuthorizationManager<RequestAuthorizationContext>` delegating check to `RequestMatcherDelegatingAuthorizationManager`, using `@EventListener` to apply the rules read once from the database and applying to `SecurityFilterChain`.
- Spring Security integrates the Spring Native for all of its authentication mechanisms and all of its authorization models (except SAML).
- **Speed it up** from `200ms` to `2ms`
- Basic authentication means the credentials are sent every single time and the password needs to be hashed every time and compared against what is in the user store (especially using the BCrypt algorithm that adds some amount of time) - switch over to a different authentication scheme, Bearer tokens as JWT tokens, bringing in the `spring-bot-starter-oauth2-resource-server` dependency (the resource server part allows to perform decoding tokens and using them as authentication mechanism) and removing `.httpBasic(Customizer.withDefaults())` with `.csrf(..)` and adding `.oauth2ResourceServer(OAuth2ResourcesServerConfigurer::jwt)` that also configures JWT out of the box.
- OAuth2 authorization server is needed to be added to mint the tokens and to give some secure keys to verify a signature on them through properties `spring.security.oauth2.resourceserver.jwt.jwk-set-uri` and `spring.security.oauth2.resourceserver.jwt.issuer-uri`.
- Finally, it is needed to define bean `JwtAuthenticationConverter` to make sure that the stored authorities in the database come back and match when a token is decoded.
- **Debugging** Spring Security application is easy through `org.springframework.security=TRACE` logging level.
- `FilterChainProxy` is the entry point and the first place that Spring-secured interceptor requests fall in and then come to the `SecurityFilterChain` and the further filters that either call the next filter or terminate the request by interrupting ~ [Chain of Responsibility](https://en.wikipedia.org/wiki/Chain-of-responsibility_pattern) design pattern.
- **Testing** is also easy in `@SpringBootTest` and `@AutoConfigureMockMvc` using `@WithMockUser(username, authorities)` annotation and static helpers in `org.springframework.security.test.**` packages.

### Impression ⭐⭐⭐⭐⭐
- ✅ Well-prepared, exhaustive and entertaining role-played scenario securing application step-by-step, key takeaways summary at the end
- ⛔ CSRF demo showing requests and responses is difficult to follow and could be explained better

______

## [Test-Driven Security](https://springone.io/2021/sessions/test-driven-security)
> "Feature development is guided by writing failing tests first and then writing the minimal amount of code necessary to make a test pass."
- Length 22:25, watched on 2021-09-08, **#spring #security #test**
- Eleftheria Stein-Kousathana as Software Engineer, VMware
- Track: Intermediate/Advanced Spring
- Language: English 🇺🇸

### Keynotes
- Dependency `org.springframework.security:spring-security-test` brings helpers in `org.springframework.security.test.**` packages and more:
  - `mockMvc = MockMvcBuilders.webAppContextSetup(context).apply(springSecurity()).build();` using autowired `WebApplicationContext`
  - `get("/greeting").with(user("Ria")).with(csrf()).andExpect(..)..`
- `String greeting(@AuthenticationPrincipal(expression = "username") String username)` injects in the currently logged user's username and `String greeting(@AuthenticationPrincipal CustomUser user)` to injects in a subtype of `UserDetails`.

### Impression ⭐⭐⭐⭐⭐
- ✅ Simple introduction to Spring security testing, TDD approach, OWASP mentioned
- ⛔ Session labeled as *Intermediate/Advanced Spring* track should include a sample of OAuth2 testing, and quite a short talk (22 mins of 30 mins available, other speakers use around 25-26 minutes)

_____

## [Code Wars: Database Decisions for Application Development](https://springone.io/2021/sessions/database-decisions-for-application-development)
- Length 51:14, watched on 2021-09-09, **#spring #security #test**
- Jennifer Reif as Developer Relations Engineer, Neo4j
- Track: Beginner-Friendly Spring
- Language: English 🇺🇸

### Keynotes
- Databases
  - In long-term is the right tool for the right job worth for future maintenance/improvement efforts
  - In the short-term forces data into an unnatural format, confuses data model, and delegates business questions to complex queries, data storage can impact application development
- Spring Data provides annotation-based mapping for POJO domain classes, repository support via interfaces, and DSL queries for each datastore
- MariaDB as an example of a relational database model through Spring Data JPA dependency
  - `orders(orderId, orderDate)`, `products(productId, productName)` and `orderProducts(quantity, unitPrice)` tables representing an M:N relationship between `orders` and `products`.
  - The concepts are `@Entity`, `@Table`, `@Id`, `@Column`, `@OneToOne`/`@OneToMany`/`@ManyToOne`/`@ManyToMany`, `@JoinColumn` JPA (`javax.persistence`/`jakarta.persistence`) and Spring Data annotations and `CrudRepository<E, ID>` interface with `@Query` annotation using JQL/HQL as a domain-specific language for querying from the database.
  - Relevant properties are `spring.dtasource.**` and `spring.jpa.**`
- MongoDB as an example of a document database model through Spring Data MongoDB dependency
  - `order(_id, orderId, orderDate, Product(productId, productName, unitPrice, quantity))` nesting structure.
  - The concepts are `@Document`, `@Id ObjectId objectId`, `@Field` Spring Data MongoDB annotations, and `CrudRepository<E, ID>` interface with `@Query` annotation using Json Structured queries (SQL works also) as a domain-specific language for querying from the database.
  - Relevant properties are `spring.data.mongodb.**`
- Neo4j as an example of a graph database model through Spring Data Neo4j dependency
  - `order(orderId, orderDate)` and `product(productId, productName)` nodes with the association `INCLUDES` from left to right between them having `unitPrice` and `quantity` attributes.
  - The concepts are `@Node`, `@Id`, `@Relationship` and `@TargetNode` Spring Data Neo4j annotations and `CrudRepository<E, ID>` interface with `@Query` annotation using Cypher as a domain-specific language for querying from the database.
  - Relevant properties are `spring.data.neo4j.**` and `spring.neo4j.**`

### Impression ⭐⭐⭐⭐☆
- ✅ Implementation of the same conceptual data representation in various database models, sorcery that programmed code on the fly worked always at the first try
- ⛔ Missing introduction of at least basic examples of use-cases for what each data model is suitable or not, more detailed comparison aside from implementation is missing

_____

## [Spring Data JDBC: Beyond the Obvious](https://springone.io/2021/sessions/spring-data-jdbc-beyond-the-obvious)
> "Strong Aggregates as the main concept of Spring Data JDBC: Whatever is reachable from the root of the aggregates is part of that aggregates and gets persisted/loaded with that root"
- Length 52:39, watched on 2021-09-09, **#spring #data #jdbc**
- Jens Schauder as Staff Engineer, VMware
- Track: Intermediate/Advanced Spring
- Language: English 🇺🇸

### Keynotes
- Spring Data offers a common abstraction for various kinds of persistent stores. The abstraction means that things look similar and it's by no means that it's possible to just swap just one database out and another one in, otherwise the common set of features would be limited and the underlying technology features are no blocked - things looks similar so working with one gives an easy way in the other. Spring Data is famous for the ability to define repositories as interfaces conceptually from the domain-driven design.
- Spring Data JPA is far more popular than Spring Data JDBC but it brings a problem that is very complex ex. it tries to map a graph of objects/classes to a graph of tables with no boundaries (lazy vs. eager) and it is needed to know what is behind saving and what is saving and what is controlled with cascade annotations.
- Spring Data JDBC is yet another support for relational databases, such as Spring Data JPA but without JPA, the key to its simplicity are strong aggregates, whatever is reachable from the root of the aggregates is part of that aggregates and gets persisted/loaded with that root just as it is kind of prescribed by domain-driven design the concept of aggregates comes from.
- **User-Defined IDS**
  - If we call `CrudRepository#save` on the entity, it set its `@Id` to the particular value that is not present in the database, it fails since `UPDATE` is executed instead of `INSERT` (because `@Id` is filled) and results in 0 updated rows.
  - Solution is autowiring and calling `JdbcAggregateTepmlate#insert` that is used under the hood. Another solution is defining a bean `BeforeSaveCalback<Minion>` that generates for example `UUID` ID for the entity if it has not set ID yet.
- **JSON / Custom Conversions**
   - We can persist an entity with an object property having further properties as JSON.
   - To write, implement `Converter<MyEntityData, JdbcValue>`, annotate converter with `@WritingConverter`, and store as `JdbcValue.of(json, JDBCType.VARCHAR)`/
   - To read implement `Converter<JdbcValue, MyEntityData>`, annotate converter with `@ReadingConverter`, and read from JSON
   - It is needed to create a configuration class (annotated with `@Configuration`) extending from AbstractJdbcConfiguration` overriding and registering a bean of `JdbcCustomConversions`.
- **Bidirectional Relationships**
   - In the relationship 1:N `Minon` has `Set<Toy>`, the full-args constructor is annotated with `@PersistenceConstructor` to mark it for Spring Data and set a reference for each `Toy#setMinion` to `this`, and that reference in `Toy` must be `@Transient`.
   - Alternatively it is possible to use `AggregateReference<Minion, Long>` in `Toy` and use `@Query` in the `CrudRepository<Toy>` to get `Collection<Toy> by `Minion#getId()` from its `AggregateReference`.
- **Caching**
- Just use Spring Data caching mechanism enabled by `@EnableCaching` and placed `@Cacheable` annotations.
- **Eager Loading References**
   - To load data in a single statement it is possible to use a view such as `ToyView extends Toy` to simply include all `Toy` fields and embedded `Minion` field using `@Embedded(onEmpt = Embedded.OnEmpty.USE_EMPTY, prefix = "minion_")` annotation and fetch them in a repository using `@Query` with a `JOIN statement`.

### Impression ⭐⭐⭐⭐⭐
- ✅ Very informative session about not-too-known Spring Data JDBC, easy-to-understand examples
- ⛔ -

_____

## [Microservices Testing at Scale](https://springone.io/2021/sessions/microservices-testing-at-scale)
> "Contract testing allows API producers and consumers to work in a decoupled fashion"
- Length 22:58, watched on 2021-09-09, **#microservice #test**
- Kishore Kotaas as Sr Architect, Discover Financial Services
- Sindhu Nair as Principal Value Stream Architect, Discover Financial Services
- Track: Architecture
- Language: English 🇺🇸

### Keynotes
- Testing monolithic architecture heavily relies on End-To-End testing and prolongs testing cycle
- Testing microservice architecture involves testing a lot of small moving pieces but system integration becomes more complex
- Unit testing (isolation, mocking, and stubbing) ->  Contract testing (contract creation and verification) -> System integration testing (system entry points) -> Backwards compatibility testing (two-step process) -> Performance testing (virtualize dependencies, short intervals, and quick feedback) -> Vulnerability testing -> -> Disruptive testing (dependency and API outage) -> E2E testing -> Browser compatibility testing (Selenium) -> Production Smoke testing (certificates, network connection)
- For disruptive testing is possible to use [Spring Boot Chaos Monkey](https://github.com/codecentric/chaos-monkey-spring-boot)

### Impression ⭐⭐⭐☆☆
- ✅ Interesting overview of the extended testing pyramid
- ⛔ Too much theoretical and abstract, missing real-live examples of what exactly is tested in each part

_____

## [A Spring Data’s Guide to Persistence](https://springone.io/2021/sessions/spring-datas-guide-to-persistence)
> "Spring Data is a familiar and consistent programming model that respects store-specific traits"
- Length 53:54, watched on 2021-09-10, **#spring #data**
- Christoph Strobl as Spring Data Engineer, VMware
- Track: Beginner-Friendly Spring
- Language: English 🇺🇸

### Keynotes
- Spring Data is not a silver bullet (doesn't manage indices), is not a magical tool, and is not one API to rule them all.
- Spring Data module anatomy starts with Repository Interface with a default implementation.
  - In the case of JPA uses Entity Manager.
  - In the case of NoSQL stores and modules it sits upon a Template API that takes care of all the resource and transaction management.
    - It uses the *Mapping* layer responsible for converting domain entities to something that can be stored via the driver.
    - For some specific properties (for example `enum`) that the driver is not understood, there is a Conversion engine for type translation.
- All of the above sits on top of the database driver and does all the heavy lifting.
- `Repository` ->` CrudRepository` (`findAll` /` findById` / `count` /` save` / `delete` / ...)>` PagingAndSortingRepository` (`findAll (Page / Sort)`)
- Derived Fetch Queries, some data sources might need a little help with `@ Modifying` annotation for` UPDATE` / `DELETE` (might return` void` / `long` /` List <E> `for none, count or modified entities respectively.
    - `List <E> findXXX`: It fetches all matched entities which puts a lot of pressure on the memory and runtime, alternatives are below.
    - `Page <E> getXXX`: Pages has set a chunk of data giving a defined rate range of matching entities and count, however, it needs to allocate resources every time the method is invoked.
    - `Slice <T> queryXXX`: WOrks like Pagination, but it doesn't know the total number of available pages (overhead of extra query) and only knows whether the next slice is available or not.
    - `Stream <E> searchXXX / streamXXX`: Streaming is the alternative for continuous scrolling, however, calling` limit` or `skip` on Stream contradicts its benefits and it is needed to close the Stream properly to release the boundary sources and free memory.
    - `Flux <E> findXXX` is an alternative for the reactive world.
- For read-operation, it is possible to use DTO Projection, Closed Interface Projection (interface with getters), or Open Interface Projection (interface with getters annotated with `@Value (" {# target ...} ")`.
- Query By Example (`List <E> findAll (Example <E> probe)`) is a good fit for web from search binding.
- Spring Data JPA has auditing support through `@ CreatedDate` and` @ LastModifiedDate` annotations and even adds who created/modified the entity if the information is provided through the implementation of Auditor and Spring Security has already implemented for it so it's only needed to plug it in and activate auditing.
- Spring Data MongoDB has `@DBRef List <Employee>` and `@DocumentReference Manager` which is a native storage format for references instead of whole documents, analogically the Spring Data JPA uses` @Embedded Manager` (possibly is needed to use `@ AttributeOverrides ({}) `to avoid field names clashes) to flatten the mapped entity.
- Spring Data JPA provides access to Stord Procedures, which is a piece of functionality stored in the database, through `@Procedure (" Employee.increaseSalary ")` for the JPA-stored procedure having both input and output parameters.
- Spring Data MongoDB has support for geospatial queries returning a result list including the distance from the target location and the average distance from all the found documents to the target location, ex. `GeoResults <E> findByOfficeLocationNear (Point p, Distance max)`.
- There is always support for native queries if a derived method is not enough, such as `@ Query` for Spring Data JPA or` @ Aggregation` for Spring Data MongoDB.
- Spring Data offers to add store-specific custom implementation using Fragment interfaces on top of `* Repository` interfaces, ie to provide implementation and extend within the repository interface that is looked for at the application start-up.
- To tune performance, Spring Data offer * Repository Metrics *, * Logiles *, * Network Stats *, and * Query Planners *.

### Impression ⭐⭐⭐⭐⭐
- ✅ Comprehenisle dive into the anatomy of the Spring Data module and relational and document data storage
- ⛔ The very same deep comparison of a graph database model (Neoj4) would be great, troubleshooting part was too way brief, and nothing about named queries as promised

_____

## [Live Coding Spring Data Queries to the End of the Persistence Universe](https://springone.io/2021/sessions/introduction-to-spring-data)
> "The queries must flow"
- Length 55:32, watched on 2021-09-11, **#spring #data**
- Greg Turnquist as Principal Software Engineer, VMware
- Track: Beginner-Friendly Spring
- Language: English 🇺🇸

### Keynotes
- Spring Data JPA has pre-baked `JpaRepositoy` that extends `PagingAndSotringReporitory` from Spring Data.
- For debugging, enable `spring.jpa.show-sql=true` and `logging.leel.org.springframework.data=TRACE`.
- Having a 1:N relationship between Manager and Employee `entities` using Spring Data JPA:
  - `List<Employee> findByNameContainingIgnoreCase(String partialName)` for full-text search.
  - `List<Employee> findByManagerName(String managerName)` query navigates across relationships.
- Use `@EnableJpaAuditing` and register `@EntityListeners(AuditingEntityListener.class)` on the `Employee` object to enable auditing through `@CreatedDate` and `@LastModifiedDate`.

### Impression ⭐⭐⭐☆☆
- ✅ Auditing introduction, very beginner-friendly
- ⛔ Since beginner-friendly the database structure could be introduced (especially how auditing stores additional data)

_____

## [Leap Ahead with Redis 6.2](https://springone.io/2021/sessions/leap-ahead-with-redis-62)
> "The 'Most Loved' database in StackOverflow's Developer survey for the 5th year in a row"
- Length 26:11, watched on 2021-09-11, **#spring #data #redis**
- Brian Sam-Bodden as Developer Advocate, Redis Labs
- DaShaun Carter as Partner Solution Architect, Redis
- Track: Beginner-Friendly Spring
- Language: English 🇺🇸

### Keynotes
- Redis (162 clients in 50 languages) stores data in memory, not on disk, which brings <1ms latency
- Spring Data is a family of project giving a Java/Spring idiomatic ways to access data from low-level constructs to high-level OO abstractions in either non/reactive or functional way
- Spring Data Redis provides easy configuration and access to Redis through low-level connectivity via Lettuce & Jedis libraries, provides `RedisTemplate` as a high-level abstraction for Redis operations (Ops), and implements key-value mappings and repositories.
- String: ValueOperations can be performed through `StringRedisTemplate#opsForValue` and the maximum size of a Redis Key is 512MB and the Redis value is 512MB
  - `redis-cli set stringKey stringValue` (`SET`) sets a key-value.
  - `redis-cli get stringKey` (`GET`) gets a value by key.
  - `redis-cli getset stringKey stringUpdatedValue` (`GETSET`) gets a value by key and sets the value immediately in one operation.
  - `redis-cli getdel stringKey` (`GETDEL`) gets a value by key and deletes the key immediately.
  - `redis-cli getex stringKey ex 3` (`GETEX`) gets and expires a key in a certain number of seconds.
  - `redis-cli set stringKey stringValue exat 1662163200` (`PXAT`) sets and expires a key at the sprcifiec Unix time in seconds.
  - `redis-cli set stringKey stringValue pxat 1662163200000` (`PXAT`) sets and expires a key at the specific Unix time in milliseconds.
  - `redis-cli ttl stringKey` (`TTL`) returns the remaining time to live of a key that has a timeout.
- Hash: HashOperations (`HSET`/`HMSET`/`HGETALL`)  can be performed through `StringRedisTemplate#opsForHash`, the hash maps identified by *keys* between string *fields* and string *values* closely resembles Java Map and can store over 4 billion field-value pairs.
  - `redis-cli hset hashKey currentTime "${date}"` (`HMET`) sets a field in the hash stored at the key to value.
  - `redis-cli hmset hashKey status "Good" name "Redis" greeting "Hi"` (`HSMET`) sets multiple fields in the hash but is deprecated as of Redis 4.0.0 in favor of `HSET`
  - `redis-cli hget hashKey greeting`  (`HGET`) returns the `value` associated with `field` in the hash stored at key.
  - `redis-cli hgetall hashKey`  (`HGETALL`) returns all fields and values of the hash stored at key.
  - `redis-cli hrandfield hashKey 4 WITHVALUES` (`HRANDFIELD`) returns an array of random distinct fields (if positive count) or random fields with possible duplicates (if negative count).
- List: ListOperations can be performed through `ListOperations<K, V>` and they are implemented in Redis as a linked list but has enough commands to turn it into a stack, queue, or any linear storage and store over 4 billion entries.
  - Adding: Pushing in `LPUSH`/`LPUSHX`/`RPUSH`/`RPUSHX`, inserting before/after `LINSERT`, and setting the value at an index `LSET`.
  - Removing: Popping off `LPOP`/`RPOP`/`BLPOP`/`BRPOP` (including blocking operations), by value `LREM` and by index range `LTRIM`.
  - Accessing: By index `LINDEX` and by range `LRANGE`.
  - Between sits: Last from one/to fill in another `RPOPLPUSH`/`BRPOPLPUSH` and pop and then push `LMOVE`/`BLMOVE` (including blocking operations).
- Set: SetOperations can be performed through `SetOperations<K, V>` and they are a collection of unique and unsorted string elements supported by operations such as union, intersection, and subtraction, most operations perform in constant time (`O(n)`).
  - Use cases: unique item management, tracking OPs, content filtering.
  - Adding `SADD` and removing `SPOP`/`SREM`.
  - Accessing `SMEMBERS`/`SRANDMEMBERS and retrieving `SSCAN`.
  - Set info `SCARD`/`SISMEMBER`/`SMISMEMBER` and set operations `SDIF*`/`SINTER*`/`SUNION*`/`SMOVE`.
- Sorted Set operations can be performed through `ZSetOperations<K, V>`, they are weighted sets, tuples with a *value* and a *score*, and elements are always taken by their score or in ranges, in spring Data Redis uses `Set<TypedTuple<E>>` data type.
  - Use cases: Priority queues, low-latency leaderboards, or secondary indexing in general
  - `redis-cli zadd game1 100 "Frank" 740 "Jennifer" 200 "Pieter" 512 "Dave" 690 "Ana"` (`ZADD`)
  - `redis-cli zrange game1 0 -1 withscores` (`ZRANGE`)
  - `redis-cli zinter 2 game1 game2 withscores` / `redis-cli zinter 2 game1 game2 withscores aggregate max` (`ZINTER`)
  - `redis-cli zdiff 2 game1 game2 withscores`
  - `redis-cli zadd game1 100 "Foo"` (`ZADD`)
- Geo: GeoOperations can be performed through `StringRedisTemplate#opsForGeo`, it is a sorted set as a latitude and longitude encoded into the score of the sorted set using the geo-hash algorithm.
  - Since it is still a sorted set, it is possible to use `Z*` commands
  - `redis-cli GEOAD running-poi -94.238226 39.029377 "Lake"
  - `redis-cli GEODIST running-poi "Lake" "Park"
- Streams before Redis 6.2 could be only trimmed to an exact or approximate number of entries which was odd as it defies stream processing
   - The rule of thumb is that each entry in a stream must have a unique ID greater than any previously seen in the stream (Redis by defaut uses milliseconds timestamps for this) and now allows you to trim based on ID.
- Redis team is up to extending and complementing Spring Data Redis with:
- Access to module commands via Spring's Templates, multi-model object-mapping support, JSON object-mapping, and RediSearch integration, Redis Graph oriented-mapping, RediSearch integration for existing Redis Hash mapped entities.
- Redis Modules Templates follow Spring Data Redis `opsForXXX()` pattern and provide a Native way to interact at the command level with RedisSON, RedisGraph, RediSearch, RedisAI, RedisBloom, and RedisTimeSeries

### Impression ⭐⭐⭐⭐⭐
- ✅ Enthustiatic talk covering wide-range of Redis topics with practical examples with some ease
- ⛔ Some commands could be omitted in favor of where Redis aim now as said at the end of the session

_____

## [Winning the Lottery with Spring: A Microservices Case Study for the Dutch Lotteries](https://springone.io/2021/sessions/winning-the-lottery-with-spring)

> "Microservices architecture built using state-of-the-art Spring Boot and Cloud components"
- Length 27:12, watched on 2021-09-12, **#spring #microservices**
- Joris Kuipers as CTO, Trifork
- Track: Architecture
- Language: English 🇺🇸

### Keynotes
- A case study of the integration platform developed for the Dutch Lotteries
- Architecture: Separate domains (verticals - specific games, subscriptions, players...) and service types (horizontals)
- Project Setup: Every service is Spring Boot or Cloud app running on AWS EKS as AWS proprietary Docker orchestrator (K8S) using blocking HTTP for inter-service communication (started at the end of 2017, but too early for reactive programming as Spring was starting too, even though it would have been a good fit since asynchronous non-blocking is the bread and butter of building gateways and integrated solutions).
- Currently around 30 services ad a bunch of libraries are inside of a single GIT repository with a single Gradle build that produces all of the actual Docker images because it is easy to build shared libraries used by a variety of services so no artifactory is needed. 
  - `libs` module contains only Java libraries (not Dockerized services): `accoung-status-store-client`, `auto-parameter-store-config`, `common-error-handling`, `common-potcodeservice-client`, `encryption`, `experience-web-shared`, `gateway-logging`, `gateway-monitoring`, `gateway-specification`, `gateway-testing`, `gateway-utils`, `http-client-autoconfiguer`, `open-api-specifications`, `sqs`, etc...
  - `inlane`, `marketing`, `players` (sample submodules: `player-experience`, `player-experience-spec`, `player-igaming`, `player-process`, `player-specs`, `player-system`, `player-system-client`, etc...)
- **Autoconfiguration for the people**
  - Spring Boot autoconfiguration is the main and most visible feature used extensively within the framework but not restricted to Spring Boot itself.
  - Although it seems like a black box or magic it is nothing more than conditional configuration classes providing beans that may or may not be initiated at startup based on certain conditions (classpath presence, something defined...), automatically applied and listed in `META-INF/spring.factories`.
  - Custom autoconfiguration benefits in encapsulation and dynamic configuration (conditions, overridable defaults) and making components auto-configurable with default properties enable configuration options discovery (`@ConfigurationProperties` allows IDE auto-completion).
  - Key concepts: `@Configuration`, `@PropertySource(value="classpath:httpclientlogging.properties")`, `@Import(HttpConnectionPoolHealthIndicaor.class)`, `@ConfigurationProperties("http.client"` on the properties POJO class, and `@Bean` definitions including `@Primary`, `@ConfitionalOnMissingBean` and `@Order`.
  - Examples: Custom JSON marshaling configuration, error handling (involves JSON response parsing), authentication (OAuth bearer token, basic auth), etc...
- **Observability for messaging**
  - Distributed Tracking is allowed by Spring Sleuth that propagates correlation ID per logical request called Trace ID and is instrumented by many Spring components out of the box.
  - Spring Cloud AWS for SQS integration (point-to-point solution - templates for sending, listener container for receiving) + Sleuth integration for message headers = To correlate asynchronous logging as a port of regular flow and provide Admin tool to link error logs for dead-lettered messages
- **Spring Cloud Netflix**
  - Part of the start of Spring Cloud allowed Netflix OSS stack to be used with Spring Boot (Eureka, Zuul, Ribbon, Hystrix...), but Netflix has stopped maintenance, and Spring support announced to stop as well providing alternatives.
  - `Experience API` -> `Process API` -> `System API` - sometimes the Process API needed to do actual work and sometimes, however, just proxy through so they wanted to have an automatic way of doing that proxy which is what Zuul did
  - With replacing deprecating Zuul they were forced to call `Experience API` -> `System API` directly in some cases, but they needed something to proxy 3rd party libraries, so they used Spring Cloud Gateway MVC (not Spring Cloud Gateway) which is a simple `RestTemplate` wrapper (`ProxyExchange passed to controller method allows for adding headers & query params, changing path and making the actual request) with Spring MVC integration for building proxies supporting reactive as well.

### Impression ⭐⭐⭐⭐⭐
- ✅ Great use-case talk especially about technology and know-how of using custom Spring Boot autoconfiguration and replacing Spring Netflix
- ⛔ Lack of time for a more detailed API gateway description and circuit breaker solution

_____

## [Live Coding Spring, Kafka, & Elasticsearch: Personalized Search Results on Ranking and User Profile](https://springone.io/2021/sessions/spring-kafka-elasticsearch)
- Length 26:42, watched on 2021-09-13, **#spring #elasticsearch**
- Erdem Günay as CTO, Layermark
- Track: Architecture
- Language: English 🇺🇸

### Keynotes
- ElasticSearch-based indexed search using analyzers and filters with a boost by popularity and by user behavior.
- `GET /_cat/indices` returns all the indices
- `POST /content/_search` queries the `content` index but an exception is thrown if the index is not found (`PUT /content`/`POST /content/_bulk`).
- **ElasticSearch Analyzers**
  - By default, ElasticSearch finds by an exact match, to enable easy search using a single letter ignoring accented characters (`é`, `í`, etc...) it is needed to use ElasticSearch Analyzers utilizing `POST _analyze` with `"tokenizer": "standard"` and `"char_filter"` with `pattern_replace` "type` to replace anything that is not an alphanumeric character.
  - To get rid of capital letters and non-ASCII characters, it is needed to add token `"filter" : ["asciifolding", "lowercase"]` and a specific `edge-ngram` among them.
  - It is needed to delete the former index and recreate the index.
  - Each `hit` has a `_score` that sets the element order in the returned structure.
  - For search by fields, it is possible to add *boosting*, ex. boost the search of artist name `artist_name` by a factor of 5 (exact match should have a bigger score) as `artist_name^5` or `artist_name.prefix^1` where are the generated tokens stored. 
  - `"fuzziness" : 1` enables to match other elements (ex. `"query": "sezan"` would match `Selena Gomez` with a low `_score` since there is a partial match in individual letters from search (basically allows typos).
- **Boosting results by popularity**
  - If the search is based on a single letter (`s`), `Shakira` might be placed below `Selena Goméz` although the popularity says otherwise (I like Shakira more, though). It is needed to enable scoring on a search through `POST /content/_search` and provide `"script_score"` in `"functions"` in `"function_score"` in `"query"`: `"script" { "source" : "Math.max(((!doc['ranking'].empty ) ? Math.log10(doc.['ranking'].value) : 1), 1)", "lang" : "painless" }`.
  - Assuming the popularity is updated programmatically (200 asynchronous hits by Kafka) it is needed to process the listen-event messages and place them in listen-event indices using `POST /listen-event-*/_search/`. User profiles are also getting generated (`POST /user-profile/_search`).
 - **Boosting by user behavior**
   - If a particular user searches for a certain element, that element should be bosted in the search for that particular user only. 
   - Another function must be taken into account similarly as previous boosting: `"script" : { "source" : "params.boosts.get(doc[params.artistIdFieldName].value)", "lang" : "painless", "params" : { .. } }`.

### Impression ⭐⭐⭐⭐☆
- ✅ Informative overview of what is ElasticSearch capable of, although, the live demo is impossible to follow but still impressive
- ⛔ The way result popularity in real-time was updated from Kafka was not clearly explained, it's not clear why Kafka figures in the demo if an easier approach could be used and the title is misleading then, data structure could be shown as not everybody has experience with ElasticSearch (all because I guess mostly caused by of lack of time)

_____

## [Debugging Complex Issues in Web Applications](https://springone.io/2021/sessions/debugging-complex-issues-in-web-applications)
> "It is often required to simulate lost connection at some point by literally two machines and "pulling out the cable."
- Length 51:15, watched on 2021-09-14, **#spring #tomcat**
- Mark Thomas as Staff Engineer, VMware
- Track: Intermediate/Advanced Spring
- Language: English 🇺🇸

### Keynotes
- **Complex issues** are subjective (everybody has a different understanding o this term), and three factors are not completely independent but it tends one dominates more than the other.
  - Issue that isn't 100% repeatable which typically means harder to debug, it drags the process out (get data, analyze, fix, repeat).
  - Only occurs under load, which generates an awful load of application/debug logs, Wireshark, and network traces.
  - Issues around concurrency tend to happen when multiple threads are interacting and a problem only occurs when a particular sequence of events happens between those threads.
  - Methodology: Identify at a high level, record the state before/after and check the consistency of them with expectations, sometimes it is needed to record multiple points.
    - To defy the statistical variation, it is needed more samples, load, and tests: at least 20 tests, at least 5 passes, and at least 5 failures, and keep adding tests and load until you meet all three.
    - Beware and the issue can have multiple root causes.
- **Use-case: [Large and concurrent HTTP/2 responses](https://tomcat.markmail.org/thread/texcre345tmyn337)** - well-described, 1-2 days to fix
  - Trouble with HTTP/2 (HTTP/2 connections are multiplexed: Multiple streams are trying to write and semaphore ensures only one writes at a time) during bulk data transfer (server -> client), multiple streams on same connection blocked indefinitely (configured an infinite timeout, so blocked until connection timeout).
    - > When a write operation is stuck servlet is not able to push any data to the client and the client is also stuck waiting for more data. There wasn't any error/exception at the client/server. `streamReadTimeout` and `streamWriteTimeout` are configured as `-1` so they are infinitely waiting for the write semaphore.
    - Described details for a test case to be coded: writing large files (1GB - 5GB) on three or more concurrent streams.
    - Described working HTTP/1.1 and non-working configurations (HTTP/2), reproducible both on blocking and non-blocking API
  - Identify root cause process:
    1. Since fairly reproducible, it was possible to continually exclude functionality to narrow the focus: Disabling asyncIO proved it is where to start looking and provided a user a workaround (disable this functionality).
    2. It was possible to see threads waiting for semaphore (it should be released by Poller indicating ready to write), code review started (possible root cause was non-volatile `interestOps` flag) but volatile `interestOps` on a higher level of tests didn't show the issue was fixed as the test was failing - the importance of sufficient testing sample.
    3. Next step was to debug Socket/Poller interactions but added logging changed time timing and the issue became less repeatable so the logging strategy needed to be changed: copy relevant information to variables and log them after failure or event of interest that much less likely affects timing - but after a log of debugging Poller was working correctly.
    4. Poller was signaling write was possible but `OperationState` was `null` which was the potential root cause because the event couldn't be processed and semaphore was never released - although it was fixed, since reading and write operations are similar, the same error could exist elsewhere (read also affected but nobody hasn't stumbled across it yet).
    5. Fix: https://github.com/apache/tomcat/commit/92b91857
- **Use-case: [Connection drops before writing response](https://tomcat.markmail.org/thread/bf6oz7ibxccvodd2)** ~ well-written report but, the presenter had no access to the system where the issue could be created, 6 weeks to fix
  - Very occasionally Tomcat didn't send a response shown in the access log, with no exceptions and Wireshark shows the GET request was followed by a TCP FIN packet from Tomcat (clean TCP close).
  - Identify root cause process:
    1. Asked various questions to try to eliminate features and/or possible failures: small response ~1kB (small enough to buffer entirely), typical response time 60m (not timeout-related), FIN sent 100µs after request received (no timeout-related), the request was fully sent (no waiting for the rest of the request and not malformed), User-agent -> Firewall -> Nginx -> Tomcat, HTTP/1.0 request (ruled out HTTP/2), no indicator from network traces from Tomcat and Nginx, unique request IDS aided correlation across logs, issue started in the last month but no obvious changes released, systems were lightly loaded (20 requests/s).
    2. Configuration changes: Switching from BIO to NIO didn't fix the issue (not in endpoint-specific code, less likely JVM issue),  added `%b` configuration to access log to suggest JSP is generating response (it was), no GZIP (no compression involved), no obvious explanation.
    3. Custom debug code to provide detail on when things were happening (who is closing the socket) because it was closed long before Tomcat tried to write, but neither Tomcat nor the application was closing it - what the hell was it?
    4. After more logging, it showed the exception "Bad file descriptor" was swallowed, because it was assumed to be a dropped client connection (Tomcat changed to debug-log them), no indication file descriptors ran out, no other connections present between Nginx and Tomcat when the issue occurred and no indication of JRE mishandled file descriptors.
    5. `strace` time showed the socket close came from somewhere in the JRE and an attempt to correlate with thread dumps to identify where the close occurred showed a native library incorrectly managed the file descriptors associated with a fork and closed a file descriptor twice - in same cases the descriptor has already been re-used for the network connection which was hence closed.
    6. Vendor accepted the native library (PDFTron) was at fault and provided instructions to disable the use, but Tomcat recommended switching to HTTP/1.1 for the Nginx/Tomcat connection to assure fewer and more persistent new connections do not constantly change the file descriptor so the native library was less likely is going to have the same one and then close it on you.
- **Use-case: [Response write does not compile](https://github.com/spring-projects/spring-framework/issues/26434)** ~ originate on Spring Framework's issue tracker, well-written, 6 weeks to fix
  - A small number of response writing fails to complete with WebFlux on Tomcat under load, low repeatability was the biggest issue as it was timing-sensitive.
  - Multiple issues identified: Spring handling of failed flushes, incorrect Tomcat error handling (attempted to flush the error page content after an I/O write error overwritten the original one, IO errs were not triggering to the error listener, Tomcat assumed `IOEception` would be seen by the container but WebFlux swallowed them).
  - After fixing the Spring issue, Tomcat now calls an error listener before internal error handling and it ended with [JDK bug](https://bugs.openjdk.java.net/browse/JDK-8263243) and [Ubuntu bug](https://bugs.launchpad.net/ubuntu/+source/linux/+bug/1924298) because for once incoming connection there were two firings of the socket accept method and there should be a one-to-one mapping (so two threads were processing the same socket).
- **Techniques**
  - Logging and Wireshark should use a 5-minute rolling window, don't be afraid to use `ERROR` logs, the network latency-related issues can be simulated in the supervisor, choose the load generator carefully as they are not always completely spec-compliant and might behave not the way you think (especially HTTP/2), it is often required to simulate lost connection at some point by literally two machines and "pulling out the cable", test on multiple platforms since VM or bare metal seems to be less of an issue.

### Impression ⭐⭐⭐⭐☆
- ✅ Impressive walkthrough of debugging truly complex issues around Tomcat including network communication or Ubuntu, and great explanation of the steps that proceeded.
- ⛔ All issues were well-written and an example of a poor one would be nice, the lip-smacking was very intensive and annoying with all due respect to the speaker.

_____

## [Spring Boot—Production Boost](https://springone.io/2021/sessions/spring-boot-production-boost)
- Length 26:09, watched on 2021-09-14, **#spring #kubernetes**
- Thomas Vitale as Senior Software Engineer, Systematic
- Track: Beginner-Friendly Spring
- Language: English 🇺🇸

### Keynotes
- If Flyway should be used with a Reactive application, it is needed to provide a JDBC connection to Flyway as it doesn't support R2DBC drivers.
- **Spring Actuator**
  - `management.endpoints.web.exposure.include=*` exposes all endpoints, although it is better to make a selection
  - `GET /actuator/health` is a base health endpoint including components (Database), liveness, and readiness needed especially for Kubernetes.
    - Liveness if `DOWN`, Kubernetes restarts the container because it means it entered into a faulty state
    - Readiness if `DOWN` means that the application cannot handle more requests so Kubernetes stops sending traffic to that specific instance
  - `GET /actuator/flyway` returns all the information regarding the migrations, stored in database relation `flyway_schema_history` with all the migration statuses that have been run.
  - `GET /actuator/prometheus` returns useful metrics about the application easy to scrap from the Prometheus server and show them in dashboards such as Grafana.
  - `GET /actuator/heapdump` creates a snapshot of heap memory to investigate ex. memory leaks and fix memory issues.
- **Packaging** (Gradle is in examples but for Maven it works the same) 
  - `./gradlew bootJar` packs the application as a fat jar, a standalone jar with all the dependencies needed by the application to run correctly with no external dependency except the JVM, which is easily deployable to cloud platforms like Heroku or Azure.
  - To make the application even more portable and deployable on a platform like Kubernetes, it is possible to package the application as a container image using `./gradle bootBuildImage`.
  - Spring Boot Plugin uses under-the-hood cloud-native build backs which is a specification to convert application source into container images without a need to provide a Dockerfile (Spring uses `packeto-buildbacks` implementation to produce production-ready images good for security and optimized for both building and running).
  - *Java Memory Calculator* is included in the final image and configures heap and non-heap memory of the JVM running in the container at start-up.
 - **Properties configuration**
   - Property files for a local development environment but Spring Ecosystem provide also has different strategies
   - A good strategy is that property files define the default value used in the deployment environment (URL to the local DB), for all properties not related to the infrastructure used Configuration Services like Spring Cloud Config (connection pools, timeouts, and retries, feature flags, external services with URLs, usernames and passwords, or PAAS specific properties), and Kubernetes specific properties with Spring Active Profiles and internal services (URLs, usernames, and passwords) use K8S Config Maps and Secrets. 
   - **Configuring Resources for JVM containers**
     - CPU: Is a compressible resource and throttles when its limit is hit - application still runs.
     - Memory: It is not a compressible resource and is OOMKilled when its limit is killed - application crashes
     - It is recommended to set in `containers` K8S YAML configuration `resources.requests.memory` and `resources.requests.cpu` and `resources.limits.memory` to assign minimum values to the container - it is also a good practice to set `requests` and `limits` values equal to guarantee the best performance.
     - To get some start-up boost it is possible to omit the CPU limit as long as we know it is a compressible resource.
   - Remember to set liveness and readiness probes in K8S YAML configuration `containers.livenessProbe` and `conainers.readinessProbe` - especially `httpGet.path`, `httpGet.port`, `initialDelaySeconds` and `periodSeconds`.
  
### Impression ⭐⭐⭐⭐☆
- ✅ Handful overview of Spring Kubernetes and production friendly features that Spring Boot Actuator provides out-of-box.  
- ⛔ The application could be ready to save some time (although the gist of the talk is to highlight quick rollout to production).

_____

## [How to Use KPIs in an Agile Delivery Environment](https://springone.io/2021/sessions/how-to-use-kpis-in-an-agile-delivery-environment)
> "Goodhart's Law: 'When a measure becomes a target, it ceases to be a good measure'"
> 
> "'A wealth of information creates a poverty of attention' - Herbert A. Simon"
- Length 24:15, watched on 2021-09-14, **#agile #project #management #kpi**
- Arijit Sarbagna as Director - Agile & DevSecOps, Atos
- Track: Agile Leadership
- Language: English 🇺🇸

### Keynotes
- Measuring in an Agile environment is problematic as businesses have been curious to measure a few specific elements: *scope* delivered on *time*, on *spec*, and on *budget* without compromising quality -> golden triangle.
- Time has changed but basic needs remain valid, we have to improve and change in perspective: *what* should be measured, *how* to be measured, and more importantly *why*?
  - **What**: Identify that helps to deliver on time, remove waste, improve quality, reduce cycle line, increase customer satisfaction, stay ahead of the competition and most importantly make/save more money.
    - Goodhart's Law applies: "When a measure becomes a target, it ceases to be a good measure" - Cobra effect is related.
    - Cobra effect is that a well-intentioned measure can often backfire and have the opposite effect to intended as happened in India - Intention: Reduce cobra population -> Action: A bounty for dead cobras -> Effect: People start cobra farming (increased population).
  - Once What is identified, derive **How** having a *Goal* -> *How* do we achieve it -> *How* do we measure it - Example: We want to deliver on time:
    - ⛔Work extra hours -> Log hours/swipes
    - ⚠️ Drive 'good estimation' -> Track committed vs. delivered user stories
    - ⛔Add more people/teams -> Scaling numbers (of teams/members), how quickly they get in track
    - ⚠️ Introduce test automation -> Automation coverage
    - ✅ Reduce 'cycle time' -> Control charts
    - ⛔ Identify 'defects' early -> Defect count in development environment 
    - ✅ Identify dependencies early -> Backlog scoring
  - **Why** do we measure what we measure?
    - We want to avoid knowing too late, or too little (to solve the root of the problem rather than symptomatically) and we want to know the right things and most importantly, we want *to do something about it*.
- Measurement should be done with specific views:
  - **Productivity**: Are we improving our ability to *deliver* products over time? - Change in amount of working product delivered per Sprint.
  - **Value delivery**: Are we *prioritizing* the right features to deliver first? - Business value per unit of a team effort.
  - **Quality**: Are we meeting our *quality* standards? - Defect rate or service downtime.
  - **Sustainability**: Are we working in a way we can continue *for the long* run? - Mental well-being and technical debt.
- If we look at measures using **Correct perspective** (the customer/consumer perspective), we can replace KPI with **CPI** (Customer Performance Indicator), i.e. how the customer would benefit:
  - Productivity -> **Reduced Costs**
  - Value delivery -> **Optimal Features**
  - Quality -> **Better Product**
  - Sustainability -> **Continuity**
- Executive Dashboard example:
  - **Wrong**: Story completion itself doesn't make sense as 3 teams are covered delivering in 4 different sprints, two chats are portraying the same information (defect patterns and cumulative story points vs. defects), pie charts with colors misinterpret the meaning
  - **Correct**: Velocity delta (velocity as points against sprints), revenue delta (revenue per story point against time) happiness delta (subjective happiness against time).
- To use KPIs correctly, identify project/program objectives and goals, set few but "well thought out" measures (not becoming targets) and make them transparent, and review them periodically (do they allow us to drive corrections/improvements) and rinse & repeat.
  
### Impression ⭐⭐⭐⭐⭐
- ✅ Highly educative and well-presented approach to the KPI/CPI with examples. Two on-spot quotes.
- ⛔ -

_____

## [Why Every Software Team Should Have a Designer](https://springone.io/2021/sessions/why-every-software-team-should-have-a-designer)
> "There are high chances we don't yet know the full scope of value that design can deliver."
- Length 24:15, watched on 2021-09-16, **#agile #project #management**
- Antonia Horvath as Delivery Lead & Design Manager, VMware Tanzu Labs
- Track: Agile Leadership
- Language: English 🇺🇸

### Keynotes
- Design altitude were design delivers value: **Surface** (look), **Structure**, **Strategy**, **Big picture**
  - Visual design (Surface + small part of Structure), User Experience (Surface + Structure), Product Design (Surface + Structure + Strategy), Strategy Design (Structure + Strategy + Big Picture).
- **Balanced Teams**: From day one of when a product is kicked off, designers, product managers, and software engineers work hand in hand, so they share accountability for the overall outcome, not only their discipline - each one is a core partner in the overall success from the day zero.
- 7 things that will change for the better when we have a designer on our team:
  - They can teach us to *listen* with humble curiosity, and with the genuine intention to *change our minds* based on what is said.
    - They can help us prevent building stuff that no one will use through *lab engagements* to run user research every one or two weeks including every single member of the team - listening users get to learn how to ask open-closed questions and interact with users.
    - Listening to users makes one so humble and makes one see how often the assumptions about this idea thought to be true aren't true at all.
  - They can bring *meaning* to our work by helping us * empathize* with the people we serve.
    - User research participants can make the whole team realize the product they are building can spark the kind of like behavior change in people which is incredibly powerful.
    - Bringing meaning into the center of our team by empathizing with the users.
   - They take chaos* and bring *order* to it as they are trained to turn uncertainty and complexity into human solutions.
     - Every product starts with such uncertainty and chaos.
     - For example, Covid-19 tracking application: Designers collaborate with the engineers, architects, and scientists to come up with the kind of like messaging logic of who and when would be pinged under extreme circumstances, i.e. so many edge cases, dependencies, and daily changing official guidelines - the result is an application so easy to use for users.
   - They are great at recognizing *when change is needed* and can optimize a team's processes and ways of working.
     - It is not only about the use of interfaces but also internal team and organization processes and seeing what can be changed for the better.
  - They are *great facilitators* as they can enable a large group of people to do their best thinking, and synthesize those perspectives into actionable insights.
  - They can help us change the world as their designs can spark impactful * behavior changes* in people.
    - For example, one wants to visualize data but the people that we need to input the data aren't the people that benefit from it, such as *timesheets* - behavior change and making sure people that people stick with it is a part of the product and that's when a designer can make a huge impact. 
  - They can help us tell stories & communicate in a way that *inspires* our audience.
    - They are great writers and UX copywriting is a whole discipline in itself so the way that the text in an application is written matters so much but it's not only text but also telling stories through images - a team would never be short appealing mockups.
- How to bring *designer* closer to the team? Rather than just go off and hire a designer follow a couple of concrete steps beginning with making engineers friends with a designer expand the cycle because people who we surround at work matter.
  1. Make our team's assumptions explicit about the software about to be written
  2. Learn about, and introduce user research in our team as it is very simple
  3. Run a design studio (at least a scathing session) for the next product challenge or new feature kick-off

### Impression ⭐⭐⭐⭐☆
- ✅ A mind-opening presentation about how a designer can be helpful with a team and organization.
- ⛔ Works with false assumptions and premises that all software engineers are extroverts and love spending time daily in the office, the talk could be more remote-friendly due to the Covid-19 situation (and international remote workers).

_____

## [How to Start Your Application Modernization Journey](https://springone.io/2021/sessions/how-to-start-your-application-modernization)
> "Don't be afraid to try different approaches to refactoring to determine what works."
> 
> "Functional *alignment* of the squads for refactoring brings *stronger outcome benefits*."
- Length 25:43, watched on 2021-09-19, **#agile #organization #learning #microservices**
- Steve Hawkins as Sr. Manager Converged Infrastructure, BT
- Track: Agile Leadership
- Language: English 🇺🇸

### Keynotes
- **BT's (company name) transformation** to remain relevant and competitive is modernizing the organization and architecture.
  - Accelerate transition and adoption of modern methods to become more responsive to customer needs as well as remove complexity and legacy to reduce time to market.
  - The organization is changing to a flatter, more accountable structure and is pivoting to tribes/squad structures to enhance decision powers.
  - Drive towards major Public Cloud adoption (SaaS), however, there was a bit of hesitancy and uncertainty from a security perspective. 
  - In practical terms: Simplify the architecture (customer journies, system interactions), modernize the application estate, establish a new operating model, introduce agile working practices and remove legacy.
- **Problem statement**: Months of analysis to clearly understand the impacts on the IT estate, ability to realize cost savings for well-defined and realizable plans, and modernization needed traction.
- **Tribe overview**: Opportunities (establish management), Cost and Plans (overall plans, decommissioning, timing), Knowledge Repository (aggregate application knowledge, automation for data sources, reporting), Refactoring Outcomes (disaggregation to microservices, decommissioning outcomes, single prioritized backlog, community) and Decommissioning Outcomes (delivery of outcomes, KPI with a single backlog).
- **Flow of the work**: Taking application in the Opportunities squad, looking at it from the EA roadmaps for categorization trying to analyze the estate to establish the right group of applications, and gradually filtering it out so at the end of the pipeline we end up with a refactoring candidate or potentially decommissioning candidate.
  - Decision trees and multiple views of a point such as costs or people effort associated with these applications, time to refactor, complexity, value delivered, and to deliver.
  - Refactoring technology approach takes a functionally discrete slice (from a set of functionalities so it can be easily refactored) and rebuilds as a microservice delivering a decoupled and resilient service. 
- **Scaling the work**: Establish multiple squads on a per application bases and leverage best practices, patterns, and methods.

### Impression ⭐⭐☆☆☆
- ✅ A complex session covering the code part of modernizing and also the people, processes, and kind of more a holistic approach, the speaker is a true professional in what he does, watching for the second time makes everything more sense, extracted two on-spot quotes defining this talk
- ⛔ Overly academical resulting in a hard focus, no definition of modernization, extremely abstract terms (examples needed), unfriendly slideshow throwing tons of small text with each slide, vague shortcuts (EA, BAU, CoE, SA)

_____

## [Staying Ahead of the Curve](https://springone.io/2021/sessions/staying-ahead-of-the-curve)
> "Create a culture of continuous learning in our environment."
- Length 54:20, watched on 2021-09-22, **#agile #organization #learning**
- Trisha Gee as Lead Java Advocate, JetBrains
- Track: Beginner-Friendly Spring
- Language: English 🇺🇸

### Keynotes
- Developers like to update to the latest and greatest technologies because it's fun to do, and it's hard to be immune to this disease, For example, applying a new technology results in the application would look like before but hopefully it might have slightly better performance, however:
  - We can't measure performance until it's implemented.
  - New technologies have limited documentation.
  - I wanted to use a niche implementation... if I succeed, I'd be *the expert*.
- **Why** - *"Fear of missing out"* leads us, so we should forget all of that, release the fear, and think of the real reasons:
  - **For the business**
    - Some technologies gain popularity and some eventually die off, which is good news as we don't need to learn all technologies to make a decision on which ones to use going forward. 
    - Invest time in two or three technologies to see how they work and observe which stick around for a longer time, so pick up them in a new project as they become more relevant.
    - For example, a data set is irregular and a relational database is not suitable to represent these data drives a need to learn a document database technology like MongoDB or a graph database like Neo4j where relationships are more important than the data itself.
    - *Approach*: Build spikes/prototypes and start using non-production code first (build, deploy, CI/CD, test) such as internal tools or a new project/service, and it's important to share the knowledge and possibly get the experts if needed.
  - **For the team**
    - Usually, releases are painful and lengthy, and introducing the correct tools and processes reduces the time and manual work, development costs, and team frustration - it is also about mindset.
    - Testing is hard and inconsistent, introducing a correct tool can help to produce more readable, expressive, effective, and well-documented tests.
    - *Approach*: Build spikes/prototypes and start using non-production code first (build, deploy, CI/CD, test) such as internal tools or skunkwork projects (hack days) that might or might not prove valuable in time (developer plugins, new products...).
  - **For you**
    - *Reasons*: I want to have fun, I want to be a technology guru in my job, I want a new job, I don't want to be left behind...
    - It is important to focus on technologies that are more important to us than we need them, we don't have to learn everything right now just in case we need it.
    - *Approaches*: Blogs, tutorials & videos, online events & streams, user groups, online courses, books, pet projects, join an open-source project, find a project at work or get a new job.
- **Developers and business needs don't match**, the approaches for the business and the team overlap themselves but not for ourselves, because we want to learn a new technology personally and not build a new production service, so how do bridge the gap?
  - *"Create a culture of continuous learning in our environment"* to bridge the gap between the developers and the business needs.
  - Protected time for learning, brown bags/lunch & learn / book clubs, user groups, hack days, skunkworks, **20% time**, conferences.
  - The bottleneck is not what we type but learning, it is discovery, and figuring out what is going on, so it is needed to learn outside the scope of our particular codebase.
- **Rule 20% of time** says we should have dedicated 20% of our working time to self-education where developers don't do what business wants them to do, but there is a lot of value to it because developers will be doing something that might have value to the business later or might have a value to the team because we can work on things like continuous delivery or deployment pipeline.
  - **Risks**: Some organizations are not necessarily sold on investing this sort of time in these activities.
    - If they upskill the developers, the upskilled developers will up and leave.
    - A higher risk is not giving them training and space to grow and learn, they will leave anyway.
  - **Benefits**:
    - Doing these activities would more likely retain developers and the organization will have highly skilled ready to adopt the right tool at the right time.
    - Happy developers will more likely stay in the organization and contribute as fully as they can.
- As a developer, don't panic, although coming to the conference might be overwhelming, try to write down the stuff that is interesting to us.
 
### Impression ⭐⭐⭐⭐⭐
- ✅ An helpful presentation providing reasons and approaches to why, where, and how should we learn new technologies to not panic. 
- ⛔ I still panic.

_____

## [A Tour of the Modern Java Platform](https://springone.io/2021/sessions/post-event/a-tour-of-the-modern-java-platform)
- Length 57:11, watched on 2021-09-22, **#java #spring #docker #containers #graalvm**
- Bruce Eckel as President, Mindview LLC
- James Ward as Developer Relations Engineer, Google Cloud
- Track: Architecture
- Language: English 🇺🇸

### Keynotes
- **Java 11+ features**:
  - **Records** are fancy immutable data structures with an auto-generated constructor and a form of getters accessing the data. 
    - Sadly it has no `copy` method in case we need to create the same record with just one changed property and another constructor is required.
  - **Text blocks** enable working with built-in new lines.
  - **Memory compaction through an array of records** as it represents just a bunch of data: `var points = new Point[] {point1, point2};`.
  - **Enhanced null pointer exception** with a helpful message describing what exactly cannot be read and why (what is `null`).
  - **Sealed classes** to allow the compiler to ask you if you have covered all the cases through `permits` in the `sealed` class.
    - This feature interacts well with a `switch` statement as a defined set of permitted subclasses is final and known on compilation time - **Pattern matching** that is exhaustive.
    - The implementations must be `final` or `sealed` to not break the definition hierarchy of sealed classes.
  - **Smart casting** simplifies the `instanceof` syntax: `if (robot instanceof Vacuum v) { v.suck(); }`.
- **Kotlin:**
  - Question mark operator (ex. `data class Bar(@Id val id: Long?, val name: String)`) says a field can be `null` and works as a sentinel or indicator on compile-time when we attempt to access a field from where is `null` allowed. 
  - Kotlin is null aware on compile-time, but in Java, it is handled in runtime.
  - Kotlin introduces *co-routines* (`kotlinx.coroutines.*` package) for reactive programming through ad-hoc polymorphism - it works as a suspendable function that can release the control to a scheduler that finds another co-routine ready to run in a lightweight manner allowing millions of them. 
  - `suspend` keyword to a function allows a function to be paused and resumed at a later time. 
- **Test Containers** help to alleviate as much variability between local development, integration or CI tests, and production.
- **GraalVM:**
  - Spring Boot has a built-in ability to turn a source code into a container with all needed to run the application using `bootBuildImage` in Maven/Gradle (`./gradlew bootBuildImage --imageName=kotlin-bars`.
  - GraalVM and Spring Native can create a very optimized version of the application, containers are about 40 MB large only.
  - An alternative to writing Dockerfiles that are hard to maintain and write is using build packs - the Cloud Native Computing Foundation created the standard called *Build Packs* that takes any source code and turns it into a Docker container - **Paketo**.
  - A file `build.gradle.kts` configures the `bootBuildImage` task: Setting `"BP_NATIVE_IMAGE" to "1"` in `environment` turns on Spring Native and GraalVM enabling to create a native image where GraalVM is doing ahead-of-time compilation to compact it down. 
  - Reflection is heavily used by Spring and it is something that cannot be done ahead of time, so Spring introduced reflection points hooks to fit well with GraalVM.

### Impression ⭐⭐⭐⭐⭐
- ✅ Entertaining folks, their speech appears like a natural dialogue, huge code I can see well on a shaking mobile screen in a gym on a runner, live demo with GraalVM, and native images explained with ease.
- ⛔ Garbage collector news and features between Java 9 and 11 deserve more space (for example modules, and `jshell` and `jpackage` commands).

_____

## [The Art of Clean Code](https://springone.io/2021/sessions/the-art-of-clean-code)
> "'Anyone can write code that a computer can understand. Good programmers write code that humans can understand' - Martin Fowler"
>  
> "'It is not enough to write the code well. The code has to be kept clean over time... Leave the campground cleaner than you found it' - Boy Scout Rule, Robert C. Martin"
- Length 14:27, watched on 2021-09-23, **#java**
- Chiamaka Okenwa as Software Engineer, Renmoney
- Track: Architecture
- Language: English 🇺🇸

### Keynotes
- Clean code is *simple*, *understandable* and *maintainable* to care about *teamwork*, *reusability* and *growth*.
- Clean code is easy to read, focused, tested, and SOLID.
- **Naming**: Use descriptive, clear, and searchable names that can be pronounced well and according to context ~ classes, functions, variables, everything.
- **Functions**: They should be small, do one thing with as least as arguments possible, have one reason to change, and follow the single responsibility principle.
- **Comments**: Avoid commenting out code chunks and use them only as a clarification of code as code is the best documentation itself.
- **Classes**: Class name must be short, show its responsibility, and have only one responsibility and only one reason to change.
- **Tests** Should be independent of each other, fast, executed in a short time, and have one assert per test.

### Impression ⭐☆☆☆☆
- ✅ Very beginner-friendly. Two on-spot quotes.
- ⛔ Extremely short talk although the topic is rich in ideas. Nothing new compared to already well-known and widely presented blog posts. What is the real meaning behind the "one reason to change" cliché? Introducing `includeSetupAndTeardownPages` way is not a good idea as we might finally end up with `includeSetupAndRegisterAndLoginAndTeardownPagesUnformattedUTF8Encoded` etc.

_____

## [Bootiful Vaccine Scavenger: A Tale of the Pragmatic Spring Framework](https://springone.io/2021/sessions/bootiful-vaccine-scavenger)
- Length 25:30, watched on 2021-09-23, **#spring #spring-boot #spring-cloud spring-cloud-streams #rabbitmq**
- Greg Meyer as Director, Distinguished Engineer, Cerner Corp.
- Track: Beginner-Friendly Spring
- Language: English 🇺🇸

### Keynotes:
- Taking an existing open-source Python project and then enhancing it and rapidly converting it into a production-grade application with the use of Spring:
  - **Vaccine spotter** is an application that allows you to pick up a location by a ZIP code and shows all the appointments available at local retail pharmacies with external REST API.
  - **Vaccine watch** is a Python bot application to query out to a specific region for un/available appointments and publishes those results out to social media networks like Twitter or Slack.
- **JVWatch** application:
  - **Architecture**: The whole application is divided into a *Consumer* and *Supplier* on top of the common Spring Boot Configuration.
    - **Supplier** contains web clients to continuously call appointment APIs (Vaccine Spotter API and Proprietary Clinic API). The transformed business objects are handed up the stack o determine whether or not a particular appointment has already been published to our social media networks and then the state of that is stored inside Redis. A  RabbitMQ queue is fed by appointments.
    - **Consumer** consumes RabbitMQ queue to push notifications to Twitter, Slack, and Email.
    - **Spring Boot* configuration profiles and conditional beans are used to enable/disable functionality inside the application so we could deploy separate instances of the application.
    - **RabbitMQ** is used although it is a single application to break down the concern and make the application deployable.
  - **Implementation**
    - The main `JVWatchAppliatinon` class is annotated with `@SpringBootApplication`, `@EnableReactiveFeignClients`, `@EnableRedisRepositories`, and `@EnableConfigurationProperties`.
    - `RestTemplaete` class has effectively been deprecated in favor of configurable `WebClient` implementing reactive programming paradigm. Another way is using a reactive non-blocking Feign client through `@ReactiveFeignCient` annotation or Retrofit HTTP client as a part of the Spring Cloud Square project (incubator project as of the time of writing).
    - Feign client URL can be either hard coded, parameterized as a hardcoded URL, or a service name that interacts with some service discovery frameworks like Eureka.
    - Spring Cloud Streams framework can abstract us from knowing of implementation details of the underlying messaging system - the redesigned framework aligned with the Spring Cloud Functions framework which itself aligns with Java 8.
    - RabbitMQ (can be replaced with Kafka) is configured through `spring.cloud.stream.*` properties, `spring.cloud.stream.function`, `spring.cloud.stream.bindings`:
    - ```
      spring.cloud.stream.poller.fixed-delay=${jvwatch.checkTask.period}
      spring.cloud.stream.function.definition=vaccineClinigDataSupplier;vaccineClinicDataSink
      spring.cloud.stream.bindings.vaccineClinicDataSupplier-out-0.destinatnion=jvwatch-clinic-data
      spring.cloud.stream.bindings.vaccineClinicDataSink-in-0.destinatnion=jvwatch-clinic-data
      spring.cloud.stream.bindings.vaccineClinicDataSink-in-0.group=jvwatch-clinic-data-sink-group
      spring.cloud.stream.bindings.vaccineClinicDataSink-in-0.consumer.concurrency=1
      spring.cloud.stream.bindings.vaccineClinicDataSink-in-0.consumer.maxAttempts=4
      spring.cloud.stream.bindings.vaccineClinicDataSink-in-0.consumer.backOffInitialInterval=15000
      spring.cloud.stream.bindings.vaccineClinicDataSink-in-0.consumer.backOffMaxInterval=60000
      ```
    - There are defined beans `@PollableBean Supplier<Flux<ClinicData>> vaccineClinicDataSupplier()` and `@Bean Consumer<ClinicData> vaccineClinicDataSink()` where `@PollableBean` means that the supplier function gets executed on a configurable interval and its returned object then gets mapped into a messaging object that's bound to a destination like a topic ora queue in the underlying messaging system.
    - Spring Boot configuration allows configuration files with properties prefixes such as: 
    - ```
      @Configuration @Configuration(prefix="jvwatch.notifications.twitter.oauth")` @Data
      public class TwitterConfigProperties {... }
      ```

### Impression ⭐⭐⭐⭐⭐
- ✅ A very impressive tale o a real application built on top of well-suited technologies able to ship into production quickly. Introduction of Spring Cloud projects and alternatives.  
- ⛔ Incorrect usage of Stream API with a side-effect. Lack of time for deployment.

_____

## [How Spring Cloud Gateway Orchestrated Our App Modernization](https://springone.io/2021/sessions/how-spring-cloud-gateway-orchestrated-our-app-modernization)
- Length 25:16, watched on 2021-09-28, **#spring #spring-cloud #devops**
- Dodd Pfeffer as Advisory Solution Engineer, VMware
- Partha Chandramohan as Solutions Architect, AARP
- Track: Architecture
- Language: English 🇺🇸

### Keynotes:
- The decade-old application about to be modernized:
  - AARP is a nonprofit organization empowering people to *choose how they live*, advocating healthcare, social security, and health insurance, and serves more than 40 million members today.
  - DSM manages the Digital and Membership strategies for AARP including the technology and production of content on [aarp.org](aarp.org) and the AARP Now application, and strategies that help them to *acquire*, *maintain* and *bring value to members*.
- **Legacy setup** consisting of over 30 applications and monoliths:
  - *Web server* -> multiple *ELB (Elastic Load Balancer)* -> 1:1 *EC2* Tomcat Application (multiple instances).
  - No meaningful auto-scaling (it was based on CPU/Memory but not actual incoming traffic), no gateway, no throttling, and no rule-based routing...
- **Needed solution**: Migrate to modernized application *gradually without impacting* the functionality, and application metrics and with a *quick rollback strategy* to the original state, *Throttle the traffic* into the new applications incrementally and route traffic to legacy and new service *at the same time*.
- **Modernization strategy**: Break down monolithic apps (key piece), gradually peel off one service at a time, and route traffic to legacy and new services, SCG was the solution for routing, A/B testing, traffic splitting, ruling by header values.
  - **Blue-Green deployment**:
    - Outlined requirement as part of application modernization - Spring Cloud Gateway became the fundamental enabler to achieve it using header values.
    - Spring Cloud Gateway enabled quick switching and roll-back between a new service and legacy solution (50:50) for A/B testing and load measurements of the infrastructure
- **The setup**:
  - *Webproxy* -> *SCG* -> routing to *Tanzu Platform* and *Legacy platform* (through *Webserver*).
- **Pros of Spring Cloud Gateway**:
  - Developer-friendly works seamlessly with the platform, keeps things simple, easy integration, comprehensive configuration list, and avoids the need for other expensive products.
 
### Impression ⭐⭐⭐☆☆
- ✅ Great session about how Spring Cloud Gateway becomes handy for application modernization as a simple solution able to fulfill a lot of solution requirements. Interesting architecture lesson.
- ⛔ Fewer abbreviations (who knows SCG stands for Spring Cloud Gateway). Confusing speakers switching. The cons of Spring Cloud Gateway were not mentioned.

_____

## [Spring for Architects](https://springone.io/2021/sessions/spring-for-architects)
> "If you want to make somebody do something, make it easy."
> "'If you don't think managing state is tricky, consider the fact that 80% of all problems in all complex systems are fixed by rebooting.' - Stuart Halloway"
> "Architects cannot afford to be dogmatic, for example, I want my teams to write tests, so I don't care what they choose to write tests in. Do you like jUnit? Fantastic, use it. Do you like Spock? Wonderful, that's great... just because I want them to write tests."
- Length 59:45, watched on 2022-02-21, **#spring**
- Nate Schutta as Architect, VMware
- Jakub Pilimon as Software Engineer, VMware
- Track: Architecture
- Language: English 🇺🇸

### Keynotes:
- Things used to be simple, i.e. having few monoliths. Nowadays we have dozens, hundreds of services dropping daily new versions and a scattered team around the globe. Architects cannot and don't want to be involved in every single decision that teams have to make. 
  - They have to **empower** our teams to make good decisions and embrace the notion of **distributed decision-making**.
  - They have to step in and **establish principles** to put on guardrails and guideposts to help teams make good decisions. A way to go is to **leverage the power of defaults**.
- From observations, distributed systems have similar needs and a lot of things come up over and over: Monitoring, circuit breakers, consumer-driven contracts, gateways, streams, externalized configuration, functions, service discovery, load balancing, documentation -> we cannot reinvent the wheel on every single project and the focus should be led on critical design decisions while empowering teams to solve critical business problems.
- **Twelve-factor app**
  - They are characteristics shared by successful apps (by Heroku).
    1. One codebase in version control, multiple deploys
    1. Explicitly defined dependencies
    1. Configuration separated from the code
    1. Backing services are just attached resources (trivial swap out, loose coupling) 
    1. Build, release and run lifecycle
    1. Stateless (durable, not in memory)
    1. Export services via port binding
    1. Scale via process (to scale horizontally)
    1. Start up fast and shut down gracefully (all in seconds, apps need to be disposable)
    1. Dev/Prod parity (from commit to production)
    1. Treat logs as event streams (no file system)
    1. Admin tasks run as one-off processes (database migrations etc.)
  - Does an application have to be fully 12-factor compliant? Nope, but should be a goal but be also ruthlessly pragmatic. **Think of it as a continuum.** Applications need to be designed properly to take the advantage of that.
  - For greenfield applications, go cloud native and don't build a legacy.
- **Monitoring** is vital to a thriving distributed architecture to know what is going on. Four primary components: 
  - Logging in to know what happened. 
  - Tracing (correlation) -> Spring Cloud Sleuth. It covers spans, sampling, and key:value pairs, it adds trace and span IDs, and stock ingress and egress points instrumented and generated Zipkin compatible traces if desired.
  - Dashboards to view the health of service and monitor key metrics involving usually infrastructure (CPU, RAM, threads, DB connections, availability, latency, response time, etc. identified earlier as part of the SLO (service level objectives)). Also the traffic level and error-failed requests etc.
  - Alerts to alert then something goes wonky and fix it ideally before the customers even notice. It means pager duty for what there has to be clear and concise on-call duty documentation. Alerts should be urgent, actionable, and require human intervention.
    > "'We don't rise to the level of our expectations, we fall to the level of our training' - Archilochus"
  - Number of tools from Wavefront to Dynatrace to New Relic -> Spring Boot Actuator.
  - **Spring Boot Actuator**
    - It is needed to use Spring Web dependencies from Initializr to enable the HTTP communication (JMX is yet another option).
    - `/actuator/beans`: The information about beans including their scope and type provided by the application
    - `/actuator/env`: The classpath, Java vendor, timezone, OS, etc.
    - `/actuator/caches/:` The caches
    - `/actuator/mappings` The HTTP mappings
    - `/actuator/scheduledtasks`: The scheduled tasks
    - `/actuator/shutdown`: To shutdown the application gracefully
    - It is possible to include Spring Security to secure the endpoints
    - It is possible to configure the custom actuator endpoints using the annotations: `@Endpoint`, `@JmxEndpoint`, `@WebEndpoint`, `@ReadOperation`, `@WriteOperation`, etc.
    - **All endpoints are enabled but not exposed by default**, which means they are by default included by the actuator.
       ```
       management.endpoint.shutdown.enabled=true
       management.endpoints.web.exposure.include=*
       ```
- **Fault tolerance**
  - We cannot prevent failure, but we can be prepared for it.
  - How to react? Error message? Backup service? Rely on cached data? Return default answer? ... *it depends*.
  - A circuit breaker is a good way to go as it watches the calls and makes sure that something that is broken doesn't get continually called.
  - Once the failure threshold is exceeded, the circuit is open and you can't complete the circuit anymore and it redirects to a fallback mechanism. Every so often it pokes the original service if it is healthy yet, so let's back to normal and close the circuit.
  - Circuit breakers are vital for healthy microservices, easy to add and customers would thank you or they don't notice at all.
  - It is better to display the user a manual error quickly than let them wait for a long time to fail and very rarely succeed.
  - **Spring Cloud Circuit Breaker** has a consistent API and allows developers to pick the implementation: Netflix Hystrix, Resilience4j, Sentinel, Spring Retry (`org.springframework.cloud`:`spring-cloud-starter-circuitbreaker-resilience4j`).
    - All can be configured as necessary and all provide a basic default configuration.
    - Free to change value thresholds, slow call thresholds, and sliding window size.
    - [Apache Benchmark](https://httpd.apache.org/docs/current/en/programs/ab.html) is a simple command line tool for benchmarks.
    - ```
      ab -n 100 http:localhost:8080/evaluate
      ```
    - Configuring a circuit breaker is done through `CircuitBreakerConfig` with either a default configuration `ofDefaults()` or a custom one (`custom()`).
    - ```
      CircuitBreakerConfig.custom()
          .failureRateThreshold(5)                          //several consecutive failing values require to open the circuit
          .waitDurationInOpenState(Duration.ofMillis(1000)) // duration in the open state
          .slidingWindowSize(2)                             // used to record the outcome of calls when the circuit breaker is closed
          .build()
      ```
- **Event-driven architecture** has multiple event patterns. Which to choose? ... *it depends*, it's all about trade-offs.
  - Event notification (for example a new client registration):
    - Something happens and the system shouts into the void (like banging a cowbell), and the emitter usually doesn't care what happens the next. 
    - This is great for being highly asynchronous and compliant with the 0th law of computer science: High cohesion and low coupling. 
    - The downside is that it is difficult to debug, to reason about the system, and easy to lose sight of the flow - that's why monitoring is crucial.
  - Event-carried state transfer (for example a client changed his address): 
    - The event carries the detail so the event subscribers don't need to ask for the details and it is an example of "tell, not ask". 
    - It reduces latency and lowers the overhead to the source systems (it doesn't mean the data get tossed around), and receivers need to handle the state.
  - Event sourcing: 
    - We record every single state change, so it turns out that the event store is the record of truth and not the database.
    - Kafka is a friend for this as it serves as a strong audit log, allows to recreate history, and makes it easy to run hypotheticals, although evolving schemas can be painful. It is challenging to replay when we interact with outside systems.
  - CQRS as Command Query Responsibility Segregation:
    - It splits the data structure into one that reads and the one that writes, which is not necessarily event-driven per se but you sort of see it combined with these approaches.
  - **How to do distributed transactions in the cloud? They don't**.
    - A real-world example: You buy a t-shirt in a shop with a return policy. The shop doesn't keep the transaction open until the return period expires. The sale is committed, if you return a t-shirt, there is a series of compensating transactions (put the t-shirt into inventory, issue you a credit, etc.).
  - **Spring Cloud Stream** for architects that want flexibility because the architecture is often defined as the decisions that are hard to change.
    - Spring Cloud Stream allows swapping brokers and using what's right for the team, so is middleware neutral.
    - It supports as expected: Kafka, RabbitMQ (`org.springframework.cloud`:`spring-cloud-starter-stream-rabbit`), Kinesis plus various partner-maintained bits.
    - It provides a binder to the external brokers that serve as a bridge between the application and the broker.
    - It allows us to implement our binder and integration-test them.
    - Destination binder connects to your messaging system, and handles the boilerplate configuration bits, so one can focus only on the business problem.

### Impression ⭐⭐⭐⭐☆
- ✅ Great and informative content on implementing architectural patterns with Spring Boot, nice explanation of an event-driven architecture, brilliant quotes, and nice-to-listen presentation style
- ⛔ They were cut off and such a situation should have been handled better (both organizers and presenters).

_____
