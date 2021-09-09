# [Spring One](https://springone.io/)

- All sessions for free and online since the 7th of September 2021

_____

## [How To Be a Java Automated Testing Superstar](https://springone.io/2021/sessions/how-to-be-a-java-automated-testing-superstar)
> "Write automated tests until they give me the confidence to deploy PROD without manual intervention."
- Length 26:24, watched on 2021-09-07, **#architecture #testing**
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
- Length 27:31, watched on 2021-09-07, **#devops #kubernetes #cloud #native #microservices**
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
- ⛔ Missing introduction into cloud-native concepts since this is marked as beginner-friendly, too many buzzwords, .NET examples, I can't extract the gist of the talk into a single quote

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
  - The concepts are `@Entity`, `@Table`, `@Id`, `@OneToOne`/`@OneToMany`/`@ManyToOne`/`@ManyToMany`, `@JoinColumn` JPA (`javax.persistence`/`jakarta.persistence`) and Spring Data annotations and `CrudRepository<E, ID>` interface with `@Query` annotation using JQL/HQL as a domain-specific language for querying from the database.
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
- Kishore Kotaas Sr Architect, Discover Financial Services
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
