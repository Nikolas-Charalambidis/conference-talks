# [JavaDays 2022](https://www.javadays.cz/en/)

|                         |                                                | Remark                                      |
|-------------------------|------------------------------------------------|---------------------------------------------|
| Location                | 🇨🇿 Czech Republic, Prague, CineStar Černý Most |                                             |
| Date                    | November 2022                                  |                                             |
| Languages               | Mostly in Czech 🇨🇿, some in English 🇺🇸         |                                             |
| Fee                     | Yes                                            | Cca $170 (online), $255 (onsite), excl. VAT |
| Conference availability | Onsite and online                              |                                             |
| Records availability    | Limited for 1-2 weeks after the event          | Only for the registered users               |

## Attended sessions list

| Session                                                                                                                    | Tags                               | Length   | 
|----------------------------------------------------------------------------------------------------------------------------|------------------------------------|----------|
| [Keynote](#keynote)                                                                                                        | #intoduction #news                 | 46:44    |
| [Scalable backend](#scalable-backend)                                                                                      | #architecture #monolithic           | 1:00:39  |
| [Building Docker images with Spring Boot Maven Plugin](#building-docker-images-with-spring-boot-maven-plugin)              | #spring #native #docker             | 35:22    |
| [Advanced tips and tricks for productivity in IntelliJ Idea](#advanced-tips-and-tricks-for-productivity-in-intellij-idea)  | #intellij                           | 46:57    |
| [Project Loom: Virtual threads in Java 19](#project-loom-virtual-threads-in-java-19)                                       | #java #multithreading               | 43:11    |
| [Domain Driven Microservices](#domain-driven-microservices)                                                                | #domain #analysis                   | 49:24    |
| [Don't be scared of benchmarks in the development](#dont-be-scared-of-benchmarks-in-the-development)                       | #java #jmh #benchmarks             | 45:53   |
| [Tips and tricks for Java memory management](#tips-and-tricks-for-java-memory-management)                                  | #java #jvm #gc #memory             | 48:54   |
| [Experience with Spring native](#experience-with-spring-native)                                                            | #spring #native #graalvm           | 42:55   |
| [Web Services, SOAP, REST and how to design them](#web-services-soap-rest-and-how-to-design-them)                          | #rest #soap                         | 52:14   |
| [jOOQ - A bit different ORM framework](#jooq---a-bit-different-orm-framework)                                              | #java #jooq #database               | 46:50   |
| [GraalVM: Java ♥ Python ♥ Micronaut](#graalvm-java--python--micronaut)                                                     | #graalvm #java #python #polygot  | 44:33   |


_____

## Keynote

> "The Oracle Java is again available free of charge for production as of Java 17."
- Length 46:44, watched on 2021-11-12, **#intoduction #news**
- Jiří Pinkas
- Language: Czech 🇨🇿

### Keynotes
- Usage statistics:
  - **Java version**: Java 8 (37%), Java 11 (29%), Java 12 and newer (12%), Kotlin (8%), Groovy (6%), Java 7 and older (5%), Scala (3%)
  - **JRE/JDK distribution**: Oracle Java (36%), Generic OpenJDK (27%), AdoptOpenJdk (16%), Amazon COrretto (7%), Azul Zulu (6%), GraalVM (3%), Other (3%), OpenLogic JDK (2.3%)
    - The best distributions: Adoptium (Temurin) which is TCK certified and GraalVM for native applications.
    - The Generic OpenJDK has half-year validity only
    - Oracle Java is again available free of charge for production under the new "Oracle No-Fee Terms and Conditions" (NFTC) license that reverses a 2018 decision. This applies to the recently released version 17 of Oracle JDK and future versions.
  - **Microservices**: Currently transitioning to microservices (44%), We are talking about it (10%), Tried, didn't work (2%) 
  - **Framework**: 
    - Spring Boot (74%), Other (18%), Quarkus (5%), Vert.x (2%), DropWizard (1%)
    - Spring-based: Spring Boot (90.6%), Spring MVC (51.8%), Java EE 29.4%, Quarkus (10.6%), Vaadin (9.4%), Jakarta EE (5.9%), JSF (5.9%), Struts (5.9%)
  - **Virtual machine platform**: Docker (41%), Kubernetes (26%), VMware (16%), N/A (10%), Other (4%), Vagrant (3%)
  - **PaaS provider**: ASW (31%), Undisclosed (24%), Azure (14%), Google Cloud Platform (11%), Other (8%), Oracle Cloud Platform (3%), IBS (3%), SAP (2%), Pivotal (2%), VMWare Tanzu (2%)
  - **Application server**: Tomcat (48%), JBoss (15%), Jetty (13%), Other (8%), WebLogic (7%), WebSphere (5%), GlassFish (4%)
  - **Build tool**: Maven (68%), Gradle (23%), Ant (6%), Other (3)
    - Though Gradle usage is raising, it needs to be used correctly and carefully, or it gets messy and complicated.
    - Spring Starter by default switched to Gradle from Maven
  - **IDE**: IntelliJ Idea (48%), Eclipse (24%), VSCode (18%), Netbeans (6%), Other (4%)
  - **CI/CD**: Jenkins (43%), GitHub Actions (16%), Other (13%), Bamboo (7%), TeamCity (4%), Circle CI (3%), Travis CI (10%), None (10%)
  - **How many times do you commit code to CI/CD build per day**: 1 time (22%), 2 times (16%), 3 times (18%), 4 times (9%), 5 and more times (35%)
  - **Percent of GC algorithms**:
    - Java 10 and older: SerialGC (22%), ParallelGC (19%), G1 (22%), CMC (21%)
    - Java 11 and newer: G1 (68%), SerialGC (33%), CMC (4%), ParallelGC (1%)
  - **Database**: PostgreSQL (34.4%), MySQL (26.9%), Elasticsearch (18.3%), Oracle (18.3%), MSSQL (14%), IBM DB2 (12.9%), MariaDB (12.9%), MongoDB (7.5%), None (6.5%), DynamoDB (4.3%), Other (4.3%), SQLLite (2.2%), Couchbase (1.1%), Firebase (1.1%)
- **Spring Boot 3**
  - Spring Boot 3 runs on Java 17 (which is the minimum version required) and supports records.
  - New Micrometer for metrics and tracing, Spring Cloud Sleuth project becomes obsolete.
  - Java EE is no longer used in favor of Jakarta EE, which means no longer `javax` packages but the `jakarta` ones.
  - Spring Security 6 has a major change where `SecurityChainFilter` has to be used instead of `WebSecurityConfigurerAdapter`.
  - Spring Data JPA and Hibernate 6
  - AOT GraalVM support for native images making Spring Native obsolete as it was an experimental project, not it is supported out-of-the-box.
- **Java 18**
  - Multiline String, Switch Expressions, Records, Pattern Matching for `instanceof`, better NPE error messages, faster start-up, and lower memory footprint

### Impression ⭐⭐☆☆☆
- ✅ A nice and brief overview of the new and incoming technologies and upgrades as well as an overview of the usage statistics from various sources.
- ⛔ Though it is nice to know which JRE/JDK distribution the speaker prefers, no technical reasoning was provided instead. So much hate towards MySQL but no explanation. It's nice to know what offers a "killer feature", but what exactly it is? Next time less of hype, swag, and buzzwords, but more explanation.

_____

## Scalable backend
- (in original: Škálovatelný backend)

> "A universal truth about architecture does not exist and its design must be context-aware."
- Length 1:00:39, watched on 2021-11-12, **#architecture #monolithic**
- Roman Bouchner
- Language: Czech 🇨🇿

### Keynotes
- Though it is a modern concept to have multiple instances, it's required to know the main goals:
  - No downtime deployment, resiliency against HW failure, better performance (huge amount of users), and protection on high traffic.  
- Scaling doesn't mean increasing the number of nodes but minds the CPU and RAM as databases are resources demanding. Though, scaling assures high availability (HA).
- Content worth reading: https://spoilerproxy.com/ and https://goodbackend.com/.
- **Context**: Small development team (also DevOps and testing), fast-paced product, strong focus on data consistency, simple architecture, infrastructure and code, simple error codes, and their handling.
- **Rules**: Backends are stateless and all states are in the database (including the locking), backends don't call each other (how to handle 504 timeouts?).
- **Idea**: Producer-consumer architecture (the BE manages data from the FE, sends it to a queue and the BE workers process them), the results processed in 3 seconds are returned synchronously, otherwise information about an upcoming notification is offered.
- **Solution**: 
  - Scalable monolithic architecture deploying the very same configurable JAR (favors easy development) through properties `api.enabled=true` and `worker.threads=1` and more layers as the properties switch if the JAR will serve as a Worker or the API REST (Main) service.
  - In case the Main service decides it's going to take a lot of time, the request is sent into a queue from where Workers take and process them.
  - **Queue**: The queue is implemented by the PostgreSQL database as it assures the transactional manner, data consistency, and simple backups (Kafka is rather suitable for non-transactional data, for example, email notifications). The database is a single source of truth.
    - 1 record is represented by exactly one row (important).
    - Data: RequestId (for Kibana), UserRequestContext (user identification, JSON request), WorkerId, RequestParameters, State (`Waiting` -> `Processing` -> `Done`/`Error` -> `ErrorResolved`), Result, Error message.
    - `INSERT` into the database is easy, but `SELECT` cannot get everything as long as synchronization between the workers is required so the record is processed by exactly one worker only:
    ```sql
    BEGIN
    SELECT * FROM my_queue WHERE state='waiting' FOR UPDATE SKIP LOCKED LIMIT 1
    UPDATE my_queue SET state='processing' WHERE id = ...
    COMMIT;
    ```
  - The stored JSON request assures that the request can be processed by a Worker regardless of its origin as it follows a defined format.  
  - **Polling? Notifications?**: The problem was how often to poll the requests from the queue. Once a second or 10 seconds?
    - The neat solution is to notify other backends without actually calling them -> PostgreSQL notifications.
    - The PostgreSQL notifications are an in-built solution that and transactional and easy to use.
    ```shell
    pgsql NOTIFY <channel> <payload>
    pgsql LISTEN <channel>
    ```
    This can be implemented into Java by a custom implementation:
    ```java
    pgListenerService.notify("worker", "params");
    pgListenerService.addServiceListener("worker", params -> { });
    ```
  - **Database scaling for HA**: The main goal is high availability (HA), the idea behind says the dumber the database is, the easier it can be scaled. 
    - PostgreSQL is capable of having one primary database for reading and writing and a secondary one for reading only. Internally it uses WAL (Write-Ahead Logging) and physical transaction replication. Theoretically, the data can be available for reading with a tiny delay in terms of milliseconds, but it is useful for analytical and aggregation processing. 
    - In
  - **Database scaling for multiple users**: Another goal is to avoid distributed databases as the development gets complex as well as its testing.
    - The solution is to add more databases but in the way transactional communication is **never** required between them.
    - A proper sharding implementation should assure that the relevant data always stay together in a single database (one company's data are only in a single database). With a new big customer and new cloud (shard), the same architecture and software can be used.
    - It is required to implement a switch (here is possible to use Kafka, and RabbitMQ as long as the consistency is not what matters here, but a quick switching).
    - It is also recommended to use UUID to distinguish company data for easy migration across the shards.
  - **Database migration**: It is not easy to rename columns or tables and it must happen in multiple steps as long as multiple versions of the application can use the same database schema.
  - **Error handling**: There is no sophisticated error handling required as no retries are implemented, the record just fails. If a problem persists for a longer time, it's worth taking a look at it.

### Impression ⭐⭐⭐⭐☆
- ✅ Though it looked like an anti-microservice session, the reasoning was context-aware. The solutions were simple and well-explained. A proof that microservices should not be always used.
- ⛔ Some relevant code and Kibana logs (though data would be anonymized) from the project to be shown would be great.

_____

## Building Docker images with Spring Boot Maven Plugin
- (in original: Tvorba docker image pomocí Spring Boot Maven Pluginu)
> "Jib is simple and helps for transition to Buildpacks."
- Length 35:22, watched on 2021-11-12, **#spring #native #docker**
- Jiří Pinkas
- Language: Czech 🇨🇿

### Keynotes

- History:
  - 2011 - Heroku initiated buildpacks (dynos)
  - 2013 - Docker, Cloud Factory adopted Buildpacks	
  - 2014 - Spotify Docker Maven Plugin
  - 2015 - Kubernetes, Cloud Native Computing Foundation (CNCF) established
  - 2018 - Jib 1.0, Cloud Native Buildpacks, CNCF Sandbox		
  - 2019 - Podman 1.0.0
  - 2020 - Cloud Native Buildpacks -> CNCF Incubation
- Dockerfiles are no longer written by hand (though it is good to know how they work), nowadays it is mostly used the Spotify Docker Maven Plugin though there are more advanced tools: Jib plugin is the best choice for a corporate and Native (Spring Boot Maven Plugin) for hipsters.
- Spring Boot Maven Plugin is simple to use, the command `mvn spring-boot:build-image` downloads a builder image where the application is built and the result is a Docker image (it is required to have Docker installed and Docker daemon run) - the resulting image is **layered**. It is required to include the plugin:
  ```xml
  <plugin>
      <groupId>org.springframework.boot</groupId>
      <artifactId>spring-boot-maven-plugin</artifactId>
  </plugin>
  ```
  
  There is Bellsoft Liberica JDK inside out-of-the-box for an unknown reason, though there are better JDK distributions.
- **Layered image**
  - Examples from infrequently to frequently changed parts: `spring-boot-loader`, `dependencies`, `snapshot-dependencies`, `application`
  - Layers enable only the changed parts can be replaced: in case we change the `dependencies`, then at least the `spring-boot-loader` can remain the same. If we change the `application` part, only the `application` part is sent to the Docker registry or Kubernetes nodes.
  - Layered JARs, images work with JIB or Builpacks and save the time between build and deployment (network traffic between Jenkins, Kubernetes nodes, etc.)
- **Buildpacks**: Buildpacks can be browsed at: https://github.com/orgs/paketo-buildpacks/repositories?q=jre and the configuration is in the `spring-boot-maven-plugin`.
  - **OpenJ9 Buildpack**
    ```xml
    <configuration>
        <image>
            <name>TODO_IMAGE_NAME</name>
            <buildpacks>
                <buildpack>gcr.io/packet-buildpacks/eclipse-openj9:latest</buildpack>
                <buildpack>paketo-buildpacks/java</buildpack>
            </buildpacks>
        </image>
    </configuration>
    ```
  - **Paketo Builder**
    - The application build happens in the builder image, there are 3 builders out-of-the-box: `full`, `base`, and `tiny`. They differ in the number of libraries installed, though the most used one is `tiny`. It is possible to create your builder, though it is complicated and worth only for corporates where the implementation of such a builder must be certified security-wise. Jib also allows creating a custom builder more simply.
    ```xml
    <configuration>
      <image>
        <name>TODO_IMAGE_NAME</name>
        <buildpacks>
          <builder>paketo-buildpacks/builder:tiny</buildpack>
        </buildpacks>
      </image>
    </configuration>
    ```
  - The plugin also can push into the Docker registry:
    ```xml
    <configuration>
      <image> ... </image>
      <docker>
        <publishRegistry>
          <username>${docker.username}</username>
          <password>${docker.password}</password>
        </publishRegistry>
      </docker> 
    </configuration>
    ```
    It is dumb the credentials must be specified right in the `pom.xml`, though it can be passed in the command line:
    ```shell
    mvn -Ddocker.username=TODO -Ddocker.password=TODO spring-boot:build-image
    ```
- **Spring Boot 3**: The plugin is already built into Spring Boot 3:
  ```xml
  <configuration>
    <image>
      <name>TODO_IMAGE_NAME</name>
      <buildpacks>
        <buildpack>gcr.io/packet-buildpacks/bellsoft-liberica:9.9.0-ea</buildpack>
        <buildpack>paketo-buildpacks/java-native-image</buildpack>
      </buildpacks>
      <env>
        <!-- optional as long as the default values are sensible -->
        <BP_JVM_VERSION>17</BP_JVM_VERSION> 
      </env>
    </image>
  </configuration>
  ```
  ```shell
  mvn spring-boot:build-image -Pnative
  ```
  Paketo buildpacks have also CLI that can build the native images:
  ```shell
  pack build test_img --builder=paketobuildpacks/builder:base -e BP_JVM_VERSION=17
  ``` 
- **Alternatives**
  - It is still possible to write Dockerfiles (a great tutorial is at spring.io/guides/topicals/spring-boot-docker)
  - As long as we are not ready for buildpacks, Jib is a good choice as it is really easy to use (`maven jib:build`) and a subsequent transition to buildpacks is not hard. We can also use Jib without Spring Boot.
  - JLink is **not** a good alternative because it conflicts with the layered JARs concepts, as long as each application has its own JRE, so they cannot share the same layers. 
- **Goals (regardless of the technology)**: Layered images, smaller images, CI/CD image builds, distroless images
  - Distroless images are without Linux distribution and contain only the application, though there is no `bash` to use in the container, it is smaller and safe from attacks.

### Impression ⭐⭐⭐⭐⭐
- ✅ Detailed and comprehensible overview of how to build Docker images using buildpacks. Jib mentioned and offered a simple alternative.
- ⛔ I still love to write Dockerfiles, it's fun. Buildpacks are confusing in terms of underlying Java versions (compatibility matrix) and this was not explained.

_____

## Advanced tips and tricks for productivity in IntelliJ Idea
- (in original: Produktivita práce v IntelliJ Idea - pokročilé tipy)
- Length 46:57, watched on 2021-11-12, **#intellij**
- Pavel Jetenský
- Language: Czech 🇨🇿

### Keynotes
- **Navigation**: 
  - Type hierarchy (**⌃H**).
  - Last edit location (**⌘⇧⌫**).
  - Backward-forward location history (**⌥⌘←** / **⌥⌘→**).
  - Quick documentation view (**⌥␣**)(works also for XML, Dockerfile, in Windows <kbd>ctrl</kbd><kbd>Q</kbd>).
  - Find a test class or method for implementation (**⌘⇧T**).
  - Other: File structure, Declaration, and usages...
- **Opening and reading**:
  - Multicolumn edit (Mouse Middle button, or **⌥⌘⇧** and left click and drag).
  - Multiple carets (**⌥⇧** and click)
  - Quick open understands wildcard (**⇧⇧** and type `*Controller`).
  - Other: Mnemonic bookmarks, Find in the previous search (for example `pet` AND `@Entity`).
- **Debugging**: 
  - Node.js debugging (**⌃⇧** click to the `localhost` address once the application starts).
  - Debug evaluation in a full-text mode can define new variables and return them to the console (a log trick can be used with a raw `List`):
    ```java
    int a = 5;
    int b = a + 5;
    a
    ```
    This prints out the value of `a` only.
  - Other: Remote debug (`ssh -f nikolas@email.com -L 5005:127.0.0.1:5005 -N`).
- **Code writing**:
  - Live templates are context-aware (`sout`, `iter`, `psvm`, `for`, `lazy`).
  - Surround with code (`if-else`, `try-catch`, etc.)(**⌘⌥T**).
  - Show context actions (**⌥↵**).
  - Delete line (**⌘X**).
  - Duplicate line (**⌘D**).
  - Move lines up or down (**⌥⇧↑** / **⌥⇧↓**).
  - Move blocks up or down (**⌘⇧↑** / **⌘⇧↓**).
- **Plugins**:
  - Presentation assistant plugin to show the shortcuts written
  - A key promoter to suggest shortcuts for repetitive actions
  - String manipulation (hash, base64, case conversion)
- **Miscellaneous**:
  - Code → Analyze Stack Trace
  - View → Appearance → Enter presentation mode

### Impression ⭐⭐⭐⭐☆
- ✅ Perfect tips I didn't know about and I will surely use: Especially from the navigation section, and String manipulation. Suggested very plugins.
- ⛔ I expected more of the debugging tricks. RIP for the Mac users  as only Windows shortcuts were presented (though the speaker is a Windows user, he could include them.

_____

## Project Loom: Virtual threads in Java 19
- (in original: Projekt Loom: virtuální vlákna v Java 19)
> "The entire JVM was reworked to support the virtual threads."
- Length 43:11, watched on 2021-11-12, **#java #multithreading**
- Miroslav Sevelda
- Language: Czech 🇨🇿

### Keynotes
- History:
  - Java 1 - Basic support for multithreading
  - Java 5 - Thread pools, executor services, futures, callable
  - Java 7 - Fork/join framework (velmi důležitý pro virt. vláken jako scheduler pro mapování na fyzická)
  - Java 8 - Completable futures, lambda, streams
  - Java 9 - Reactive streams (against IO-bound threads)
  - Java 19 - Virtual threads
- **Current model**: In the current model, a thread in the JVM always means there is a corresponding OS thread linked. This model will be still available and unchanged with the Project Loom. 
- **Project Loom** ([JEP 425](https://openjdk.org/jeps/425)): This brings a new solution of massive parallelism and introduces virtual threads that are invisible from the point of view of the OS. It means it's possible to create theoretically billion of threads without saturating the OS. This principle is similar to what Python uses: virtual thread synchronization into a single one. This project doesn't introduce virtual threads only.
- Motto: Easy-to-use, high-throughput, lightweight concurrency, and new programming models.
- **Virtual thread** is a planned and manager thread visible only on the JVM level and is similar to the [green thread](https://en.wikipedia.org/wiki/Green_thread) concept and analogous to the currently unused POSIX threads.
  - The solution was to return to the M:N model: In this case, the JVM platform thread is mapped to the OS thread and a huge amount of virtual threads. Context switch through a scheduler mounts the virtual thread to the JVM platform thread, which is a single OS thread.
  - **Terminology**:
    - Virtual thread: - Invisible in the OS.
    - Platform thread: - JVM thread mapped to the OS thread.
    - Carried thread - Platform thread bound to the virtual thread as it is not possible to run a virtual thread with no platform thread. 
    - Thread mounting - Process when the virtual thread is assigned to platform one.
    - Thread unmounting - Process when the virtual thread is unassigned from platform one. It happens automatically as soon as the virtual thread invokes a blocking operation.
  - **Disadvantages of the current model**:
    - JVM thread is bound to the OS thread, which means the thread management is above the JVM, and thread creation is expensive. 
    - Inflexible memory allocation for the thread stack memory, which is not under the control of the JVM.
    - Problematic support for massive parallelism and not optimal for IO-bound threads that are not computing in a blocked state.
  - **Advantages of the new model**:
    - Virtual threads are inexpensive, so it's possible to create billion of virtual threads, basically as much as we need without the OS and resources limits.
    - Scheduling and memory management are under the JVM control and the GC.
    - Alternative to the Async-IO and reactive approaches.
    - No dangerous operations like suspending or stopping threads since the virtual threads are un/mounted automatically.
  - **Disadvantages of the new model**:
    - The debugging can become harder as it is no longer possible to use the debugging tools on the OS level.
    - It is too soon for comprehensible conclusions. 
- **New API**: Only a few changes were introduced for minimal interference to the existing API for sake of an easy transition to virtual threads. The new solution completes the current API design and the virtual thread is still an instance of `Thread` as well as the platform thread.
  - Each virtual thread is of a type `DAEMON` and has fixed `NORM_PRIORITY` that cannot be changed (as it never worked correctly and synchronization primitives were always a better way to go).
  - The virtual thread scheduling is implemented with the existing `ForkJoinPool` in the FIFO mode that implements the "work stealing", though it is partially customizable and it is possible to use a custom scheduler (but why). It is great that virtual threads are built on the existing and well-known implementation.
  - **New factory methods**: The old implementation is unchanged and it is needed to use factory methods to create a virtual thread.
    - `Thread vt = Thread.ofVirtual()` - creates a virtual thread
    - `Thread pt = Thread.ofPlatform()` - creates a platform thread
    - `Thread vt = Thread.startVirtualThread()` - creates and starts a virtual thread
  - **Fluent style**:
    - `Thread vt = Thread.ofVirtual().name("virtual").unstarted(runnable);`
    - `Thread vt = Thread.ofPlatform().name("platform").unstarted(runnable);`
  - **Builder and factory styles**
  - **Methods**:
    - `boolean isPlatformVirtual = Thread.ofPlatform().isVirtual(); // false`
    - `boolean isVirtualVirtual = Thread.virtual().isVirtual(); // true`
    - `boolean isVirtualDaemon = Thread.virtual().isDaemon(); // true`
  - **Executor services**:
    - `ExecutorService service = Executors.newVirtualThreadPerTaskExecutor();`
- **Antipatterns**
  - The virtual threads should not be pooled as long as they are lightweight and the pool management becomes an overhead compared to threads creation. However, there is a new dedicated thread pool `ExecutorService`, though it's better to just create a thread and let the system handle it.
  - Do not use priorities with virtual threads.

### Impression ⭐⭐⭐⭐⭐
- ✅ I don't know if I am impressed by the speaker or the topic. Disadvantages and patterns were well-explained. 
- ⛔ None about the session. I think I can give up on Project Reactor and Spring Webflux.

_____

## Domain-Driven Microservices
> "The used language should be ubiquitous."
- Length 49:24, watched on 2021-11-12, **#domain #analysis**
- Ivan Macalák
- Language: Czech 🇨🇿

### Keynotes
- Domain Driven Design is an approach to software development that helps us to break down a complex system into loosely coupled components with well-encapsulated logic and clearly defined dependencies among them. 
- It's needed to have a *strategy* that matches the architecture.
- **Domain** is a sphere of knowledge represented by the *ubiquitous language* and encapsulates a domain model and bounded context.
  - It is a conceptual model of the domain.
  - **Ubiquitous language** is important as analysts and developers should use the same language and the same terms.
    - Shared language between the business and development teams.
    - The language comes from the business and is enriched by the development team.
    - Domain dictionary defines many terms that in/directly help to form the domain.
  - **Bounded context** defined the problem boundaries (for the meaning of a given Domain Model) and enables decomposing into smaller parts.
    - Complex business domain consists of several Bounded Contexts. 
    - Each Bounded Context contains a **Domain Model**.
    - **Context Map** is a set of dependencies between Bounded Contexts, though they are encapsulated, they still need to react with each other. The Context Map gives *meaning* to Bounded Contexts.
    - For example Smart building management:
      - Building management → Occupant (Name, Floor, Flat number, Relations), Room, Energy consumption...
      - User profile → User (Name, Favourites, Contacts, Payment methods, Invoice address), Payment details, Address...
      - Incident management → Reporter (Name, Email, Phone), Issue, Elevator
      - Authorization → User (Username, Email, Password, Roles), Role credential...
      - Equipment → Sensor, Elevator, Actuator...
  - **Domain vision statement**
    - It is important to use common, factual, realistic, honest, clear, and understandable language (ex. what is the occupant).
    - Avoid superlatives, and avoid marketing and technical/implementation language.
    - There are required domain experts: Either hire an external one or train an internal employee.
  - **Contribution**: Common understanding, improves collaboration, leads to meaningful software design, and tackles complexity with a systematic approach.
- **Subdomains** are grouped into 3 categories and they interact with each other (source: https://pbs.twimg.com/media/FKIT_MnXMAYm2I7?format=jpg&name=4096x4096).
  - **Generic** does not contain anything special to the organization but is still needed for the overall solution (OSS, Identity, and Access management).
    - *Reduces integration costs* of the *supporting* subdomain: Adjusting open-source or vendor solutions is our needs become expensive, so we build it ourselves.
    - *Opportunity* to the *core* subdomain: Buidling best-in-class as-a-service solution for something eveyone was doing in-house.
  - **Supporting** is necessary for the organization to succeed, but it does not fall into the core domain category (Incident management).
    - *Commoditization* of the *generic* subdomain: Maintaining an in-house supporting tool becomes a burden.
    - *Opportunity* to the *core* subdomain: Adding new capabilities to our boring CRUD starts generating revenue.
  - **Core** is what makes an organization special and different from other organizations. An org. cannot succeed/exists without being exceptionally good in their core domain (Building management).
    - *Commoditization* of the *generic* subdomain: Switching to the open-source solution that outperforms our differentiator.
    - *Simplification* of the *supporting* subdomain: Reducing effort and simplifying it as it's not a differentiator anymore. 
- **Strategic design** (what)
  - Do we understand business processes and operations? Which operations a system has to perform to accomplish its goal?
  - The knowledge shall be acquired by both domain experts and developers.
  - **Strategic design patterns**:
    - Cooperation:
      - Partnership: `(A) --- (B)`
      - Shared kernel: `(A (  ) B)`
   - Consumer-supplier:
      - Conformist: `(A) → (B)`: `A` takes a model of `B`
      - Anti-corruption layer: `(A)[ACL] → (B)`: `B` change has no impact on `A`
      - Open-host service: `(A) → [OHS](B)`: `B` defines data exchange format (`B` provides API to `A`)
   - No-collaboration:
     - Separate ways: `(A) x (B)`
- **Tactical design** (how)
  - Defines Domain Model, Entities, Value Objects, Aggregates, Domain Events, Repositories, Services...
  - **Aggregate** is a transaction consistency boundary, that contains root entity and sub-entities, for example, floor (equipment, room (doors, windows), and additional properties)). All the aggregate components should be in the boundary of the bounded context (due to transaction reasons should not touch outside).
- **Domain model pattern**:
  ```
  project/
  ├─ application/
  │  ├─ api/
  │  ├─ service/
  ├─ domain/
  │  ├─ model/
  ├─ infrastructure/
  │  ├─ messaging/
  ```
- **Q&A**:
  - How a microservice should be big? 
    - The size is not determined by the number of lines but by the number of operations, subdomain integrations, context, etc. The Domain Driven Design reveals how the microservice will be big and not vice versa.
  - Is the Domain Driven Design a waterfall?
    - The strategic design becomes a most likely waterfall, but as long as it's flexible, agile is possible. Usually, the first 10 iterations should be in the waterfall style and the rest can be managed in an agile way.
  - Where is the boundary between Domain Driven Design and technical design?
    - There are no exact boundaries.    

### Impression ⭐⭐⭐☆☆
- ✅ A necessity of a ubiquitous language is highlighted. The session demonstrated how the Domain-Diven Design is coupled with Microservice Architecture.
- ⛔ Too theoretical and abstract, it would be nice to show a sample core, generic and supporting domain designed in detail. The relationship between subdomain categories/types was not explained at all.

_____

## Don't be scared of benchmarks in the development
- (in original: Nebojte se benchmarků při vývoji)
> "Moore's Law ceases to apply as a single core performance converges to a limit defined by the laws of physics."
- Length 45:53, watched on 2021-11-13, **#java #jmh #benchmarks**
- Jan Novotný
- Language: Czech 🇨🇿

### Keynotes
- Moore's Law ceases to apply as a single core performance converges to a limit defined by the laws of physics: Performance becomes a thing again!
  - The producers compensate for the performance limits by adding more threads.
- **Java Microbenchmark Harness (JMH)** is a low-lever test framework for simple and quick *unit* and *integration* performance tests writing.
  - Maven dependencies: `org.openjdk.jmh:jmh-core` (`compile`) and `org.openjdk.jmh:jmh-generator-annprocess` (`provided`).
  - Samples are available at https://github.com/openjdk/jmh/tree/master/jmh-samples/src/main/java/org/openjdk/jmh/samples 
  - There are three basic ways to run it:
    - Using IntelliJ Idea using a JMH plugin (click on the green triangle and run as a test).
    - Using the main class:
    ```java
    org.openjdk.jmh.Main.main(args);
    ```
    - Using the command line, for which it's necessary to use a Maven Shade Plugin (`org.apache.maven.plugins:maven-shade-plugin`) to create a fat jar (also called *uberjar*) that contains the performance tests.
    ```xml
    <executions>
        <execution>
             <phase>package</phase>
             <goals>
	         <goal>shade</goal>
             </goals>
             <configuration>
                 <finalName>benchmarks</finalName>
                 <transformers>
                     <transformer implementation="org.apache.maven.plugins.shade.resource.ManifestResourceTransformer">
                         <mainClass>org.openjdk.jmh.Main</mainClass>
                     </transformer>
                     <transformer implementation="org.apache.maven.plugins.shade.resource.ServicesResourceTransformer"></transformer>
                 </transformers>
                 <filters>
                     <filter>
                         <!-- sharding of signed JAR fails without this: https://stackoverflow.com/q/999489/3764965 -->
                         <artifact>*:*</artifact>
                         <excludes>
                             <exclude>META-INFO/*.SF</exclude>
                             <exclude>META-INFO/*.DSA</exclude>
                             <exclude>META-INFO/*.RSA</exclude>
                        </excludes>
                    </filter>
                </filters>
            </configuration>
        </execution>
    </executions>
    ```
    Upon running `mvn clean install`, the JAR with tests can be run:
    ```shell
    java -jar target/benchmarks.jar
    ```
  - **Configuration**
    - **Annotations** are available to configure the test, though they can be overridden with the command line arguments.
      - `@Benchmark` annotates the performance test itself.
      - `@Warmup` defines the warm-up.
      - `@Measurement` defines the benchmark measurement details.
      - `@Fork` defines the forking. The test should run in the separate JVM (`@Fork(1)`) to not influent the tests and yield representative results
      - `@BenchmarkMode` and `@OutputTimeUnit` to define the output.
      - `@Setup(Level.XXX)` and `@TearDown(Level.XXX)` for test and data preparations.
      - `@State(Scope.XXX)` to define the test data scope.
    - **Builder** using `OptionsBuilder` contains a context help thanks to its fluent style and using `include(String regex)` can define through CI/CD what set of tests would be run, assuming smart package naming.
  - **Lifecycle of the test**
    - There are three levels: `Level.Trial`, `Level.Iteration`, and `Level.Invocation`.
      - **Trial** is run *once* before (`@Setup(Level.Trial`) and after (`@TearDown(Level.Trial`) the test and is used for initialization and closing resources.
      - **Iteration** is run *always* before (`@Setup(Level.Iteration`) and after (`@TearDown(Level.Iteration`) each test iteration and is used for the data preparation and clean-up.
      - **Invocation** is run *always* before (`@Setup(Level.Invocation`) and after (`@TearDown(Level.Invocation`) the test method (`@Benchmark`) itself and might have an impact on the test, so it's recommended to not handle data in this phase unless it's quick compared to the test execution itself.
  - **Data preparation**
    - A stateful data object annotated with `@State` and defined scope is passed as a formal parameter to the method annotated with `@Benchmark`.
    - **Scopes** define the liveness of the `@State` data object:
      - `Scope.Thread` is the most used one and the data are isolated and instantiated per thread.
      - `Scope.Benchmark` creates one instance for all the tests and threads, so beware of the synchronization and access.
      - `Scope.Group` grants all instances will be shared across all threads within the same group defined by `@Group`. This advanced scope is the least and the hardest to use and configure correctly.
  - **Debugging**
    - The debugging of the test (especially data preparation) does not work with a JVM fork (`@Fork(1)`). For this purpose, the fork has to be disabled (`@Fork(0)`).  
  - **Gotchas**
    - It's needed to watch out for the data if they are sent with each iteration as we assume.
    - Constant folding: The compiler eliminates useless code and pre-calculates predictable results. It's needed to use a return type or `Blackhole` (can be used as a formal parameter to the `@Benchmark` method) to consume the result.
    - Safe-looping: The compiler eliminates useless iterations and does magic with cycles at all (unrolling, jamming, vectorization), so it's better to leave the iteration mechanisms to the JMH and measure only the algorithm itself.
  - **Profiles** reveal the reasoning behind the bad test results as we want to know why.
    - IntelliJ idea has its profiler displaying the process and time diagram of test method execution.
    - JMH Stack Profiling can reveal the multithreading issue, for example:
      - A single thread processes 2878000 ops/s, output:
      ```
      Stack profiler:

      ...[Thread state distributions]......
       75.0%	RUNNABLE
       25.0%	TIMED_WAITING
      ```
      - Multiple (12) threads process together each only 2121178 ops/s, output:
      ```
      Stack profiler:

      ...[Thread state distributions]......
       69.2%	BLOCKED
       24.0%	RUNNABLE
        6.7%	TIMED_WAITING
      ```
      - The reason is that the threads spend nearly 70% of the time in the `BLOCKED` state.
    - Types of profiles: Stack profiling, Linux performance profiling (for L1 cache), GC profiling, ClassProfiler (number of un/loaded classes), CompilerProfiler (time dedicated for JIT compilation)...
  - **Best practices**:
    - Define a problem, formulate a hypothesis, state the expectations and perform an experiment.
    - Ask the following: What do I try to measure? Do I measure it correctly? Why the result is not what I expect? What happens?
    - Do not stick with the absolute numbers and rather compare and use the relative numbers as the results depend on hardware, OS, surrounding code, etc.
    - Use the production-alike data.
    - Observe the `BLOCKED` thread time in multithreading applications.
    - Be careful with formulating and summarizing the results. It's worth consulting with a colleague, reviewing the test, and involving more people.
    - Observe the changes in time and use the CI/CD pipeline for the performance tests.  

### Impression ⭐⭐⭐⭐☆
- ✅ Explanation of why Moore's Law ceases to apply. Highlighted pitfalls of the data preparation for JMH tests. Nice overview of profiling and the tools for it. 
- ⛔ Rather a beginner session and a quick introduction to the JMH as most of the information can be found easily. I cannot imagine how to configure and run the JMH tests for integrations as was advised. JMH Stack Profiling was not sufficiently explained.

_____

## Tips and tricks for Java memory management
- (in original: Tipy a triky práce s pamětí v Javě)
> "The first rule of optimization is to not optimize."
- Length 48:54, watched on 2021-11-13, **#java #jvm #gc #memory**
- Petr Adámek
- Language: Czech 🇨🇿

### Keynotes
- **Cases when `java.lang.OutOfMemoryError` occurs**:
  - It's not possible to allocate a new instance of an object, because the memory runs out in the Heap.
  - A huge array is allocated that doesn't fit in the memory.
  - Native memory ran out in the Metaspace.
  - Allocation of memory failed on native code call through JNI
  - High overhead of Garbage Collector (GC)
    - By default, if Garbage Collector takes 98% or more of the JVM run and deallocates less than 5% of memory, the error is thrown
  - It's not possible to create a new thread, because the underlying OS limits the maximum number of threads (this surprisingly throws this error as JVM does not have much information from the OS).
- **Cases when `java.lang.StackOverflowError` occurs**:
  - Excessive deep or infinite recursion.
- **JVM memory management**:
  - **Heap**: Object allocation, array allocation, String pool, GC
    - The Heap is divided into 2 basic sections: Young Generation (Eden + Survival) and Old Generation
    - The GC checks the younger objects more often than the survival and old ones.
    - Most of the problems are related to Heap and Non-Heap: Although the overall memory allocated of the Heap is sufficient,`java.lang.OutOfMemoryError` is thrown when a single section gets full. For example, it doesn't matter if the remaining sections are nearly empty if the Eden section is full. 
  - **Non-Heap**: Internal data used by the JVM that are invisible to a developer (code cache, formerly Permanent Generation (PermGen), now Metaspace).
  - **Stack**: There are 2 types of stacks: A Native Stack (for native and JNI methods) and a Normal Stack (for our methods). Each thread has its stack.
    - Method calls and metadata storage. Each *frame* has: Return value, local variables, operand stack, and current class constant pool reference (into the Non-Heap memory).
- **Garbage Collector (GC)**
  - The Heap memory is hierarchically divided by young/old generation and further sub-groups for the optimized and fairly sophisticated run.
  - General garbage collecting algorithms overview:
    - **Tracing (Reachability tree)**: The GC traverses the oriented graph of objects, traces for the reachable ones, and removes the unreachable ones. Though this algorithm is slow and expensive but can detect and remove cyclical references. JVM GC uses this algorithm.
    - **Reference counting**: Counts the number of references and removes if fall to zero. This algorithm can miss cyclical references.
  - By default, the less memory is available, the more aggressively the GC runs to release the memory in the JVM. This approach delays  `java.lang.OutOfMemoryError`, though the overhead of the GC run raises and the application becomes less responsive (lags).
- **String internization** is implemented using the flyweight design pattern (referencing a shared copy).
  - String literals (those between `""`) are interned (pooled) automatically. Though we can call `String#intern`, it's not recommended for the short-lived strings as we risk wasting memory.
  - It's also not a good idea to intern the sensitive data as it's not under our control when they are removed from the memory by the GC. For this reason, all sensitive content should be passed through `char []`.
- **Java 8 changes to the JVM**
  - Permanent Generation is replaced by a more dynamic Metaspace. It caused problems with multiple hot-deploy (ex. Tomcat, etc.) when the JVM is not registered. Though a new classloader is loaded and the reference to the old one is discarded and the class references become replaced by the new one, releasing the long-living classes takes a delay (if they are released at all) and the maximum memory limit can be hit. 
  - **Permanent Generation (PermGen)** has a fixed size of an allocated continuous block of native memory in the OS that is **not** efficiently deallocated.
    - `-XX:PermSize=[size]` and `-XX:MaxPermSize=[size]` parameters.
  - **Metaspace** has a dynamically allocated memory continuous block of native memory in the OS that is efficiently deallocated as long as the OS only limits how much memory is can be provided.
    - `-XX:MetaspaceSize=[size]`, `-XX:MaxMetaspaceSize=[size]`, `-XX=MinMetaspaceFreeRatio=[ratio]`, `-XX:MaxMetaspaceFreeRatio=[ratio]` parameters.
- **Memory management problems - resolving**: 
  - Generate a memory dump for further analysis:
    - `jmap -dump:[live],format=b,file=<file=path> <pid>`
    - `jcmd <pid> GC.heap_dump <file-path>`
    - `java -XX:+HeatDumpOnOutOfMemoryError`
  - The biggest issue is that the application can become irresponsive before `OutOfMemoryError` is thrown and the critical moment is missed.
  - Restart the application:
    - `java -XX:+ExitOnOutOfMemoryError`
    - `java -XX+CrashOnOutOfMemoryError`
    - `java -XX:OnOutOfMemoryError="stop.sh %p"`
  - Use the monitoring tools: JMX, Jolokia, https://gceasy.io/ for `gc.log` analysis.
- **Memory management problems - prevention**:
  - Analyse the memory management on the production run (take off-peak load memory dumps to find out irregularities).
  - Don't forget to do performance testing.
  - Optimize JVM to not use too big Heap which increases the GC overhead.
  - Minimize the memory demand: 
    - Minimize stateful integration and HTTP session usage.
    - Make the application stateless.
    - Beware of soft/weak references in the cache and the size of the keys (it is not a good idea to put a whole request as a key).
  - A large number of hash-based structures (`HashMap` and `HashSet`) is also not a good idea and a plain array can be a better choice.
  - VisualVM is a nice tool but favors smaller Heap sized.

### Impression ⭐⭐⭐⭐☆
- ✅ Educative session about how is JVM memory management done in sufficient detail.
- ⛔ I expected more "tips and tricks", especially ineffective code snippets and how to fix them.

_____

## Experience with Spring native
- (in original: Zkušenosti se Spring Native)
> "Nobody uses Liferay and WAS today."
- Length 42:55, watched on 2021-11-13, **#spring #native #graalvm**
- Jiří Pinkas
- Language: Czech 🇨🇿

## Keynotes
- Spring Boot 3 is in its final design as Spring Native for Spring Boot 2 was rather experimental, vastly different from Spring Boot 3, and the entire implementation for native support and ahead-of-time (AOT) was 3 times reworked. GraalVM Native Support needs to be included in [start.spring.io](https://start.spring.io/).
- **GraalVM native image**
  - A technology that compiles ahead-of-time Java code into a standalone runnable application called a *native image*.
  - Such an application contains application classes, dependency classes, and classes used by Java runtime and native JVM code.
  - Native images don't run on JVM (but they come from JVM), but they load important JVM components like memory management, thread scheduling, etc. from a different runtime called Substrate VM.
  - The result application has a quick start (doesn't load classpath and classes that happen now on the build time) and consumes less RAM compared to JVM.
  - Process: Java bytecode (application, dependencies, JVM) → Native image build (static analysis finds what is used, initialization, snapshot) → Binary code (code, image heap).
  - Use cases:
    - Microservices - resulting Docker image is smaller, starts up quickly, and has a lower memory footprint
    - Serverless and CLI applications - they start instantly
  - GraalVM community version uses only the old SerialGC that is suitable only for smaller heaps, though the GraalVM enterprise edition can use G1.
- **Native and dynamic code**
  - What is saved into a native image depends on the result of the static analysis on the native image build time. 
  - Such an analysis **can't** find out the usages of JNI, reflections, dynamic proxies, or resources from classpath - such classes need to be added manually through configurations. Luckily, Spring can do that.
    ```    
    META-INF/
    ├─ native-image/
    │  ├─ resource-congif.json
    │  ├─ serialization-config.json
    │  ├─ jni-config.json
    │  ├─ proxy-config.json
    │  ├─ reflect-config.json
    ```
  - This was a huge problem since Spring Framework is built on top of reflections and dynamic proxies. The creators had to catch up with Micronaut and Quarkus and implement native image support. They originally ignored the benefits of a quick start-up, then they found out that serverless is an interesting use case and finally, they found out they are fucked up. The implementation of AOT was lengthy and reworked 3 times. 
  - GraalVM can't dynamically create runtime classes out-of-the-box.
- **Spring Boot 3**
  - It's required to have GraalVM installed as an SDK to support GraalVM.
  - The execution of `mvn clean spring-boot:build-image -Pnative` calls `spring-boot-maven-plugin:process-aot` internally that runs a Spring container and discovers what beans were created on the application load and generates the following:
    - `graalvm-reachability-metadata`: `reflect-config.json`, `resource-config.json`, etc. from various libraries
    - `spring-aot`: `reflect-config.json`, `resource-config.json` from the application
  - Spring luckily doesn't need to store all beans into such JSON configuration files, but only their definitions.
  - For example, Spring Data JPA beans are normally created on the application startup, but now it's not possible so that's why the AOT plugin was created.
  - The creators of Spring AOT found out that such an approach can be used even for non-Spring applications, so it makes sense as a slight performance and size improvement, although the native would not be used. 
- **Native executable** is no longer platform-agnostic, which is completely different from what Java was created on top of. Now the solution brings a platform-specific executable, which is ok because we have Docker and CI/CD that were not available years ago. We somehow reinvented the old solution. 
- **Comparison** (the more points, the better):
  |                    | JVM | Native | Remark                                                                        |
  |--------------------|-----|--------|-------------------------------------------------------------------------------|
  | Maturity           | 100 | 50     | JVM is a proven solution, native is pretty much new                           |
  | Build time         | 10  | 2      | What are 5 seconds for JVM becomes tens of minutes for native                  |
  | Startup time       | 20  | 100    | What are seconds and minutes for JVM is milliseconds for native                 |
  | Latency/throughput | 100 | 7      | JIT in a long run can optimize the runtime, which is not possible for native. |
  | Memory footprint   | 50  | 100    | What is 200 MB RAM for JVM becomes 50 MB RAM for native                       |
  - Build time becomes very long and it is not possible to reduce it significantly.
  - Image size is smaller for native solutions, but custom layered images are useless for native solutions because each image has a custom and optimized JDK for a given application.
  - Memory footprint is also smaller for native solutions.
- **Problems**:
  - How do we register resources, proxy classes, or classes used by reflection? A solution is to implement `RuntimeHintsRegistrar` and activate with `@ImportRuntimeHints`: 
    ```java
    public class CustomRuntimeHintsRegistrar implements RuntimeHintsRegistrar {

        @Override
        public void registerHints(RuntimeHints hints, ClassLoader classLoader) {
            hints.resources()
                    .registerPattern("banner.txt")
                    .registerPattern("static/*")
                    .registerPattern("templates/*");

            var categories = new MemberCategory[] {
                    MemberCategory.DECLARED_FIELDS,
                    MemberCategory.INTROSPECTED_DECLARED_CONSTRUCTORS,
                    MemberCategory.INTROSPECTED_DECLARED_METHODS,
                    MemberCategory.INVOKE_DECLARED_CONSTRUCTORS,
                    MemberCategory.INVOKE_DECLARED_METHODS
            };
            reflectionHints.registerType(org.thymeleaf.engine.IterationStatusVar.class, categories);
            reflectionHints.registerType(org.thymeleaf.expression.Lists.class, categories);
        }
    }
    ```
  - However, it does not import all the classes as long as some DTO/records used for reflection are ignored. There is a non-Spring workaround solution using `org.reflections:reflections`. Create a custom annotation `@RegisterForReflection`, scan and register these classes.
    ```java
    var rootPackage = Main.class.getPackageName();
    var classes = new Reflections(rootPackage).getTypesAnnotatedWith(RegisterForReflection.class)
    var categories = new MemberCategory[] { ... };
    var reflectionHints = hints.reflection();
    classes.forEach(type -> reflectionHints.registerType(type, categories));
    ```
- **Production support**:
  - [GraalVM Dashboard](https://www.graalvm.org/dashboard/) can introspect the contents of the built application.
  - [Dive](https://github.com/wagoodman/dive) can instrospect layered Docker images.
  - Actuator metrics become limited as they don't display the used memory amount. 
  - Profiling becomes problematic and Java Flight Recorder is limited.
  - **Heap size tuning**:
    - `docker run -m 200m --rm -it -p 8080.8080 <image_name> -XX:+PrintGC -XX:+VerboseGC` prints each GC run details. Currently, there is no other solution.
  - **Observation** of a sample stateless application:
    - RAM was reduced from 200 MB to 50 MD, response time got lowered from 60ms to 30ms, and start-up took only 70ms.
    - The build time increased brutally from a few seconds to 3-6 minutes.
- **Future**:
  - Native image support to be standardized in OpenJDK through Project Leyden
  - Reachability metadata repository is a repository of reflection and dynamic proxies for various projects so we would write and configure JSON configurations as least as possible. GraalVM thoroughly cooperates with Spring.
    - Link: https://medium.com/graalvm/enhancing-3rd-party-library-support-in-graalvm-native-image-with-shared-metadata-9eeae1651da4

### Impression ⭐⭐⭐⭐⭐
- ✅ Excellent understanding and experience of the speaker as well as his ability to explain simply and highlight the important aspects of the native approach. Solutions to common problems.
- ⛔ -

_____

## Web Services, SOAP, REST, and how to design them
- (in original: Web Services, SOAP, REST aneb jak je správně navrhovat)
> "Insurance companies have contracts older than 30 years that need to be supported, though the products are no longer offered. For that reason, they use old systems."
- Length 52:14, watched on 2021-11-13, **#rest #soap**
- Petr Adámek
- Language: Czech 🇨🇿

## Keynotes
- The author has experience with rather older projects as he works as a consultant for corporates.
- Law of the instrument (law of the hammer, Maslow's hammer): Is a cognitive bias that involves an over-reliance on a familiar tool: "I hold a hammer, everything becomes a nail".
- There is not a universal solution and tools, there exist limits and exceptions, and quite often.
- **SOAP vs REST**:
  |                  | SOAP                                  | REST                                            |
  |------------------|---------------------------------------|-------------------------------------------------|
  | Characteristics  | Heavyweight                           | Lightweight                                     |
  | Origin           | Specification and abstraction attempt | Organic                                         |
  | Protocol         | Any (including HTTP)                  | HTTP only                                       |
  | Definition       | WSDL (advantage in the beginning)     | Swagger (disadvantage as it came later)         |
  | Content format   | XML only                              | Any (usually JSON, sometimes XML)               |
  | Content schema   | XML schema                            | Depends on the content format (ex. JSON schema) |
  | Class generation | `wsimport`                            | `swagger-codegen`                               |
  | Operations       | Any                                   | `GET`, `POST`, `PUT`, `PATCH`, `DELETE`         |
- **XML vs JSON**:
  | Goal                 | Universal and compatible format with SGML | Human readable format                             |
  |----------------------|-------------------------------------------|---------------------------------------------------|
  | Formal standard      | XML 1.0 (1998), XML 2.0 (2006)            | RFC 5627 (2006), RFC 8259 (2017), ECMA-404 (2017) |
  | Semistructured data  | Yes                                       | No                                                |
  | Comments             | Yes                                       | No                                                |
  | Process instructions | Yes                                       | No                                                |
  | Namespaces           | Yes                                       | No                                                |
  | Schema               | XML schema, RelaxNG, Schematron           | JSON Schema                                       |
  | Transformations      | XSLT (any version), XQuery                | XSLT 3.0, jolt, jslt, JSONata                     |
- **When to use SOAP?**
  - Due to historical reasons. The other party requires it.
    - Insurance companies have contracts older than 30 years that need to be supported, though the products are no longer offered. For that reason, they use old systems. It makes no sense for such companies to rewrite the existing solutions that become deprecated with time. Also, XML structures tend to be rich and complex in definition and XML allows nesting.
  - It's needed to build something on top of the existing SOAP solution. It's needed to route through multiple nodes (SOAP is protocol-independent). 
  - It's needed to use XML, WSDL, or SOAP extensions (WS-security, WS-MeliableMessaging, WS-Addressing) or use it as a universal format.
  - Reasons XML is required: There is an existing schema to be used. Produce SOAP as a REST service. Schemes need to be combined. There is a need for semistructured data. There is a need for XSLT transformations.
- **Best practices**:
  - Contract first as it's possible to develop in parallel unless a small BE-FE application with few endpoints is developed.
  - Well-defined contract including non-standard situations and error codes. An empirical approach to how the service works is not a good idea.
  - Use standard and appropriate error codes for a particular situation (4XX and 5XX for the beginning). 
  - Think out-of-the-box and don't let the Law of the instrument influent you, for example, there are other solutions aside from REST and SOAP:
    - GraphQL
    - Messaging (JMS, Kafka, RabbitMQ, etc.)
  - Client identification and correlation ID
  - REST API versioning with backward compatibility: The approach with headers is not usually recommended and it's better to include the version to the path which is handy for future version decommissioning.
  - REST API filter: If there is required a sophisticated filter for nested projection, better grab GraphQL.

### Impression ⭐⭐⭐⭐⭐
- ✅ A great speech proving SOAP is not dead (ex. insurance industry), though shall rather not be used for greenfield projects. Well-explained comparison focusing on *when* SOAP or REST shall be used and how.
- ⛔ I would expect some design tips and tricks for SOAP as I know REST quite well.

_____

## jOOQ - A bit different ORM framework
- (in original: jOOQ - tak trochu jiný ORM framework)
> "OpenSource version is for free for the latest open source DB versions (PostgreSQL, MySQL...)."
> "It's a one-man-show project."
- Length 45:50, watched on 2021-11-13, **#java #jooq #database**
- Leoš Přikryl
- Language: Czech 🇨🇿

## Keynotes
- jOOQ /ʤuk/ stands for "jOOQ Object Oriented Querying" and is a Java framework for database integration introducing type-safe and database platform-independent SQL queries. It does *not* hide the SQL queries, unlike Hibernate, it only makes them easier to use.
- **Database integration solutions comparison**
  - **JPA/Hibernate**:
    - **Advantages**: Database platform-independent SQL. Suitable for CRUD operations and persisting complex object graphs.
    - **Disadvantages**: Extremely complex, difficult, and error-prone (lazy fetch, 1-N queries...). Not suitable for complex queries across multiple tables and the following need to be used: JPQL/HQL, Criteria API, QueryDSL (though we know how the SQL should look like, it's not easy to write it with QueryDSL), native queries... Cannot be used if the database structure is not known in advance.
  - **JDBC**
    - **Advantages**: Enables the full power of the SQL. Useful if the database structure is not known in advance. 
    - **Disadvantages**: Low-level API that is not database platform-independent and the SQL queries must follow a dialect. No type-safety and prone to SQL injection.
  - **Spring JdbcTemplate**
    - **Advantages**: Enables the full power of the SQL. Useful if the database structure is not known in advance. More comfortable API than a pure JDBC.
    - **Disadvantages**: No type safety and no not database platform independence. Errors in complex queries are rather discovered in runtime.
  - **jOOQ**
    - **Advantages**: Enables the full power of the SQL. Useful if the database structure is not known in advance. Database platform-independent SQL and type-safe.
    - **Disadvantages**: Not suitable for persisting complex object graphs. The free version works only for the latest versions of open-source databases.
- **jOOQ**
  ```sql
  SELECT last_name, first_name FROM user
  WHERE role = 'admin'
  ORDER BY last_name, first_name;
  ```
  ```java
  dslc.select(USER.LAST_NAME, USER.FIRST_NAME)
      .from(USER)
      .where(USER.ROLE.eq("admin"))
      .orderBy(USER.LAST_NAME, USER.FIRST_NAME);
  ```
  - **Database-first approach**
    - The database is a source of truth and the code is generated from it. This approach is preferred as the database changes less often than the code.
    - Developers need to design the data structure and the database becomes more efficiently used.
    - A code generator produces a Java/Kotlin type-safe code with the database description: tables, sequences, stored procedures, indexes, records
    - 
    - **Type safety**
      ```java
      dslc.select(USER.LAST_NAME, USER.FIRST_NAME)
          .from(USER)
          .where(USER.ROLE.eq(1)) // the USER.ROLE is of the type VARCHAR → compiler-time error
      ```
      ```java
      dslc.select(USER.LAST_NAME, USER_FIRSTNAME) // the USER.LAST_NAME was renamed to USER.SURNAME → compiler-time error
          .from(USER)
          .where(USER.ROLE.eq("admin"));
      ```
  - **Generator-first approach**
    - It's possible to use jOOQ even without the code generator, though it is not recommended.
    - It's useful in case the database structure is not known in advance. 
    - **No type safety**
      ```java
      dslc.select(field("last_name"), field("first_name"))
          .from(table("user"))
	  .where(field("role").eq("admin"))
	  .orderBy(field("last_name"), field("first_name"));
      ```
  - **Quick start**
    - Start with the [`DSL`](https://www.jooq.org/javadoc/dev/org.jooq/org/jooq/impl/DSL.html) to get `DSLContext` which is the main object for writing the queries.
      ```java
      var dslc = DSL.using(connection, SQLDialect.POSTGRES);
      var dslc = DSL.using(dataSource, SQLDialect.POSTGRES);
      ```
    - Spring Boot offers `org.springframework.boot:spring-boot-starter-jooq` to configure and inject the context.
  - **Queries**
    - **`WHERE`**
      ```java
      dslc.select(AUTHOR.LAST_NAME, AUTHOR.FIRST_NAME)
          .from(AUTHOR)
      .where((AUTHOR.LAST_NAME.eq("London").or(AUTHOR.FIRST_NAME.like("J%")).and(AUTHOR.YEAR_OF_BIRTH.between(1800, 1900)));
      ```
      ```java
      dslc.select(AUTHOR.LAST_NAME, AUTHOR.FIRST_NAME)
          .from(AUTHOR)
          .where(
              AUTHOR.LAST_NAME.eq("London").or(AUTHOR.FIRST_NAME.like("J%")),
              AUTHOR.YEAR_OF_BIRTH.between(1800, 1900)));
    - **`JOIN`** is supported as well as all common joins (`INNER`, `LEFT/RIGHT/FULL OUTER`, `CROSS`) and introduces *semi* and *anti* joins.
      ```java
      dslc.select(AUTHOR.LAST_NAME, AUTHOR.FIRST_NAME, BOOK.TITLE)
          .from(AUTHOR)
          .join(BOOK).on(AUTHOR.ID.eq(BOOK.AUTHOR_ID))
          .where(AUTHOR.ID.eq(1));
      ```
      ```java
      dslc.select(AUTHOR.LAST_NAME, AUTHOR.FIRST_NAME, BOOK.TITLE)
          .from(AUTHOR)
          .join(BOOK).onKey() // in case the foreign key is well-configured
          .where(AUTHOR.ID.eq(1));
      ```
      ```java
      dslc.select(BOOk.author().LAST_NAME, AUTHOR.author().FIRST_NAME, BOOK.TITLE) // jOOQ can do an implicit JOIN
          .from(BOOK)
          .where(AUTHOR.ID.eq(1));
      ```
      - **Semi-join** returns all the left-side rows for which there *exists* at least one right-sided row. It's a kind of "fake" join as it finds out whether there is something to join.
        ```java
        dslc.select(BOOK.TITLE).from(BOOK)
            .leftSemiJoin(BOOK_TO_BOOK_STORE).onKey();
        ```
        ```sql
        SELECT book.title FROM BOOK
        WHERE EXISTS (
            SELECT 1 FROM book_to_book_store
            WHERE book_to_book_store.book_id = book.id)
        ```
        ```java
        // alternative using jOOQ without the semi-join
        dslc.select(BOOK.TITLE).from(BOOK)
            .whereExists(
                dslc.selectOne()
                    .from(BOOK_TO_BOOK_STORE)
                    .where(BOOK_TO_BOOK_STORE.BOOK_ID.eq(BOOK.ID)));
        ```
      - **Anti-join** is an opposite to *semi join*. Returns all the left-side rows for which there *doesn't exist* at least one right-sided row.
        ```java
        dslc.select(BOOK.TITLE).from(BOOK)
            .leftAntiJoin(BOOK_TO_BOOK_STORE).onKey();
        ```
    - **Aggregation**
    ```java
    dslc.select(count()).from(BOOK);
    ```
    ```java
    dslc.select(avg(BOOK.YEAR_OF)).from(BOOK);
    ```
    ```java
    dslc.select(LANGUAGE.DESCRIPTION, count())
        .from(BOOK).join(LANGUAGE).onKey()
        .gropuBy(LANGUAGE.DESCRIPTION)
        .orderBy(count()).desc();
    ```
    - **Complex queries**
      ```sql
      SELECT author.first_name, author.last_name, count(*) FROM author
          JOIN book ON book.author_id = author.id
          JOIN language ON book.language_id = language.id
      WHERE lanuage.code = 'CZ' AND book.published_in > DATE '2020-01-01'
      GROUP BY author.first_name, author.last_name
      HAVING count(*) > 5
      ORDER BY author.last_name ASC NULLS FIRST
      LIMIT 5 OFFSET10;
      ```
      ```java
      dslc.select(AUTHOR.FIRST_NAME, AUTHOR.LAST_NAME, count()).from(AUTHOR)
          .join(BOOK).onKey()
          .join(LANGUAGE).onKey()
          .where(LANGUAGE.CODE.eq("CZ").and(BOOK.PUBLISHED_IN.gt(LocalDate.of(2020, 1, 1))))
          .groupBy(AUTHOR.FIRST_NAME, AUTHOR.LAST_NAME)
          .having(count().gt(5))
          .orderBy(AUTHOR.LAST_NAME.asc().nullsFirst())
          .limit(5).offset(10);
      ```
  - **Reading**
    - Single line: `fetchOne` returns one or `null` or exception in case of more rows, `fetchSingle` returns exactly one row or exception in case of more rows, `fetchAny` returns one or `null` and ignores the rest in case of more rows.
    - Multiple lines: `fetch` returns a `List`, `fetchLazy` returns a cursor (similar to JDBC `ResultSet`), `stream` returns Java 8 Stream, `fetchGroups`, `fetchMap`, `fetchArray`...
    - POJO mapping using the column names via reflection (though can be sufficient)
      ```java
      dslc.select(BOOK.ID, BOOK.TITLE).from(BOOK)
          .fetchInto(Book::class);
      ```
    - POJO mapping using the constructors is type-safe
      ```java
      dslc.select(BOOK.ID, BOOK.TITLE.as("bookTitle")).from(BOOK)
          .fetch(Records.mapping(Book::new));
      ```
  - **Writing**
    - Using SQL
      ```java
      dslc.insertInto(AUTHOR, AUTHOR.FIRST_NAME, AUTHOR.LAT_NAME)
          .values("Jack", "London")
          .execute();
      ```
      ```java
      dslc.update(AUTHOR)
          .set(AUTHOR.FIRST_NAME, "Jack")
          .where(AUTHOR.ID.eq(3))
          .execute();
      ```
      ```java
      dslc.delete(AUTHOR)
          .where(AUTHOR.ID.eq(100))
          .execute();
      ```
    - Using active record pattern
      ```java
      // CREATE
      var book = dslc.newRecord(BOOK);
      book.setTitle("1984");
      book.store();
      // ID is autogenerated and populated automatically
      var bookId = book.getId();
      // RETRIEVE
      var book2 = dslc.fetchSingle(BOOK, BOOK.ID.eq(bookId));
      // UPDATE
      book2.setPublishedIn(2000);
      book2.store();
      // DELETE
      book2.delete();
      ```
    - Generated POJO and generated DAO
      ```java
      // CREATE
      var book = new Book();
      book.setTitle("1984");
      bookDao.insert(book);
      // ID is autogenerated and populated automatically
      var bookId = book.getId();
      // RETRIEVE
      var book2 = bookDao.fetchOneById(bookId);
      bookDao.update(book2);
      // DELETE
      bookDao.delete(book2);
      ```
  - **Complex features**
    - **Emulation of non-existing database functions**, for example, PostgreSQL doesn't know `median`.
      ```java
      dslc.select(median(BOOK.PUBLISHED_IN)).from(BOOK); // there is no PostgreSQL median
      ```
      ```sql
      SELECT percentile_cont(0.5) WITHING GROUP (ORDER BY book.published_in) FROM book;
      ```
    - **Enumerations**, the database native enums can be mapped to the Java `enum`. Hibernate struggles with PostgreSQL enumerations.
      ```sql`
      CREATE TYPE book_type AS ENUM ('NOVEL', 'POEM', 'ESSAY'); -- PostgreSQL enumerations
      ```
      ```java
      dslc.celect(BOOK.TITLE).from(BOOK).where(BOOK.TYPE.eq(BookTypeEnum.NOVEL));
      ```
    - **Native database arrays**, the database native arrays can be mapped to the Java array.
      ```sql
      CREATE TABLE book (
         tags text[]
      );
      ```
      ```java
      public class Book implements Serializable { // jOOQ generated class
          private String[] tags;
          // getters and setters
      }
      ```
    - **Nested data structures** are supported in jOOQ, though Hibernate excels in it. Sadly, only H2 and PostgreSQL database support native arrays (the method `array` can be used), though in other database types the method `multiset` is a proper substitution for `array`.
      ```java
      public record Book(int id, String title) {}
      public record Name(String first, String last) {}
      public record Author(int id, Name name, Book[] books) {}
      ```
      ```java
      // this generates duplicated author first and surnames and requires further processing in Java
      dslc.select(AUTHOR.ID, AUTHOR.FIRST_NAME, AUTHOR.LAST_NAME, BOOK.ID, BOOK.TITLE)
          .from(AUTHOR)
          .join(BOOK).onKey()
          .fetch();
      ```
      ```java
      // column mapping
      dslc.select(
              AUTHOR.ID, 
              row(AUTHOR.FIRST_NAME, AUTHOR.LAST_NAME).as("name"))
              array(
                  dslc.select(row(BOOK.ID, BOOK.TITLE))
                      .from(BOOK)
                      .where(BOOK.AUTHOR_ID.eq(AUTHOR_ID))).as("books"))
                      .from(AUTHOR)
          .fetchInto(Author::class);
      ```
      ```java
      // constructor mapping
      dslc.select(
              AUTHOR.ID,
              row(AUTHOR.FIRST_NAME, AUTHOR.LAST_NAME).mapping(Name::new))
              array(
                  dslc.select(row(BOOK.ID, BOOK.TITLE))
                      .mapping(Book::class, Book::new)
                      .from(BOOK)
                      .where(BOOK.AUTHOR_ID.eq(AUTHOR_ID)))
          .from(AUTHOR)
          .fetchInto(Author::class);
      ```
    - **Format as JSON** is useful when a three-layer architecture is not required.
      ```java
      var jsonFormat = new JSONFORMAT()
          .recordFormat(JSONFormat.RecordFormat.OBJECT)
          .format(true);
      System.out.println(query.fetch().formatJSON(jsonFormat));
      ```
    - **Format as an ASCII table** is useful for debugging due to the well-overridden `Object#toString` method.
      ```java
      System.out.println(query.fetch());
      ```
  - **Other features**
    - The main use case is for a dynamic approach to the database, it can generate procedures, triggers, etc. It has a rich API over the databases.
    - Migration scripts are recommended to use and work well with jOOQ.
    - Works well with Hibernate and those can be combined over the same transaction manager. This approach is also recommended to combine various use cases where each framework excels. 
  - **Problems with Kotlin generators**
    - KotlinGenerator generates in POJO types of all database columns as nullable (correct in the principle, but troublesome in practice).
    - The solution should come with the 3.18 version.
    - An alternative is the JavaGenerator with `@Nullable` and `@NotNull`.
- **jOOQ dual license model**
  - OpenSource version is for free for the latest open source DB versions (PostgreSQL, MySQL...).
  - Paid version (99€, 399€, and 999€ per developer per year depending on the obscurity of the database) has no further fees (application, server) and supports older open source database versions as well as other non-open source databases. The paid subscription includes support.
- **Credits** 
  - **Author** of jOOQ is Lukas Eder in his Data Geekery company in Switzerland. Sadly, it's a one-man-show project but has a nice guide (https://www.jooq.org/learn/) and a blog (https://blog.jooq.org/).
  - [GitHub Copilot](https://github.com/features/copilot) can generate some easy jOOQ code from SQL.

### Impression ⭐⭐⭐⭐☆
- ✅ Amazing introduction to jOOQ so I would love to try it out immediately. GitHub copilot.
- ⛔ The transaction management (commits, rollbacks) was not explained at all as well as triggers, procedures, etc. though the session was more than rich enough.

_____

## GraalVM: Java ♥ Python ♥ Micronaut
> "It's possible to render beautiful graphs with `pygal` in Java through GraalVM."
- Length 44:33, watched on 2021-11-13, **#graalvm #java #python #polygot**
- Štepán Šindelář
- Language: Czech 🇨🇿

## Keynotes

- **GraalVM** is a universal virtual machine for running an application written in JavaScript, Python, Ruby, R, JVM-based languages (Java, Kotlin, Scala), and LLVM-based languages (C, C++). It is similar to JVM which supports native images, JIT mode, and non-JVM languages - a kind of universal swiss knife.
  - The structure is very similar to the standard JVM, but has additional tools:
    - `./bin/gu` - `gu` is a tool for installing and managing optional GraalVM language runtimes and utilities, that can be listed with `./bin/gu list`, for example, `./bin/gu install python` installs the Python language runtime
    - `./bin/graalpy` starts the Python CLI
- **GraalPy** only supports currently Max/Linux, but is compatible with CPython. Unlike JPython supports native extensions, such as NumPy, Matplotlib, etc. The peak performance is on par with PyPy (currently the fastest alternative). It also supports Java interoperability and Python venv.
- It is possible to call Python code from Java as well as Python scripts, though GraalVM doesn't support multiple return types from Python to Java.
- The GraalVM can be included in the IDE as an SDK and the GraalVM-specific classes are already a part of the SDK, so the IDE should recognize them without importing a Maven dependency. 
  ```java
  Context ctx = org.graalvm.polygot.Context.newBuilder("python").build() // part of GraalVM
  Value value = ctx.eval("python", "1+1");
  Integer i = value.fitsInInt ? value.asInt() : null;
  ```
- It's possible to get bindings from the snippet and execute them:
  ```java
  ctx.eval("python", 
  """
  def foo(a,b):
      return a+b
  import polygot
  polygot.export_value("myid", foo)
  """);
  ```
  ```java
  ctx.getPolygotBindings().getMember("myId").execute(2, 3);
  ```
  ```java
  ctx.getBindings("python").getMember("foo").execute(2, 3);
  ```
- If Python needs to access the Java arrays and classes, it's needed to allow the host access:
  ```java
  ctx.allowHostAccess();
  ```
- Sample usages: 
  - Simple and quick scripting where Python excels primarily (though alternatives are to write a Maven plugin or dependency), but this is useful for smaller companies.
  - To render beautiful graphs with `pygal` in Java through GraalVM.  
  
### Impression ⭐⭐⭐⭐⭐
- ✅ Though I am not interested in Python, the capabilities of GraalVM are fucking lit. The live coding was done well.
- ⛔ -

_____
