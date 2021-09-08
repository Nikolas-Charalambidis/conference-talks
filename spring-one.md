# [Spring One](https://springone.io/)

- All sessions for free and online since the 7th of September 2021

_____

## [How To Be a Java Automated Testing Superstar](https://springone.io/2021/sessions/how-to-be-a-java-automated-testing-superstar)
> "Write automated tests until they give me the confidence to deploy PROD without manual intervention"
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
> "Developer experience on DIY platforms is lacking"
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
- ⛔ The structure doesn't match the agenda in the introduction and a bit chaotic, rather Tanzu platform promotion, lacking expected pure K8S tips, VSCode

_____

## [Modern Application Configuration in Kubernetes](https://springone.io/2021/sessions/modern-application-configuration-in-kubernetes)
> "Spring Cloud Config vs. K8S Config-maps and secrets"
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
> "Container is process isolation"
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
> "Favour DTO interfaces projections without advanced techniques (SpEL, nested associations) for read-operations over managed entities"
- Length 54:50, watched on 2021-09-08 #spring #jpa
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

