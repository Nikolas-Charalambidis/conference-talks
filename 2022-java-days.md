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
| [Don't be scared of benchmarks in development](#dont-be-scared-of-benchmarks-in-development)                               | #java #jmh #benchmarks             | 45:53   |
| [Tips and tricks for Java memory management](#tips-and-tricks-for-java-memory-management)                                  | #java #jvm #gc #memory             | 48:54   |
| [Experience with Spring native](#experience-with-spring-native)                                                            | #spring #native #graalvm           | 42:55   |
| [Web Services, SOAP, REST and how to design them](#web-services-soap-rest-and-how-to-design-them)                          | #rest #soap                         | 52:14   |
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
  - **JRE/JDK distribution**: Oracle Java (36%), Generic OpenJdk (27%), AdoptOpenJdk (16%), Amazon COrretto (7%), Azul Zulu (6%), GraalVM (3%), Other (3%), OpenLogic JDK (2.3%)
    - The best distributions: Adoptioum (Temurin) which is TCK certified and GraalVM for native applications.
    - The Generic OpenJDK has half-year validity only
    - The Oracle Java is again available free of charge for production under the new "Oracle No-Fee Terms and Conditions" (NFTC) license that reverses a 2018 decision. This applies to the recently released version 17 of Oracle JDK and future versions.
  - **Microservices**: Currently transitioning to microservices (44%), We are talking about it (10%), Tried, didnt work (2%) 
  - **Framework**: 
    - Spring Boot (74%), Other (18%), Quarkus (5%), Vert.x (2%), DropWizard (1%)
    - Spring-based: Spring Boot (90.6%), Spring MVC (51.8%), Java EE 29.4%, Quarkus (10.6%), Vaadin (9.4%), Jakarta EE (5.9%), JSF (5.9%), Struts (5.9%)
  - **Virtual machine platform**: Docker (41%), Kubernetes (26%), Vmware (16%), N/A (10%), Other (4%), Vagrant (3%)
  - **PaaS provider**: ASW (31%), Undisclosed (24%), Azure (14%), Google Cloud Platform (11%), Other (8%), Oracle Cloud Platform (3%), IBS (3%), SAP (2%), Pivotal (2%), VMWare Tanzu (2%)
  - **Application server**: Tomcat (48%), JBoss (15%), Jetty (13%), Other (8%), WebLogic (7%), WebSphere (5%), GlassFish (4%)
  - **Build tool**: Maven (68%), Gradle (23%), Ant (6%), Other (3)
    - Though Gradle usage is raising, it needs to be used correctly and carefully, or it gets messy and complicated.
    - Spring Starter by default switched to Gradle from Maven
  - **IDE**: IntelliJ Idea (48%), Eclipse (24%), VSCode (18%), Netbeans (6%), Other (4%)
  - **CI/CD**: Jenkins (43%), GitHub Actions (16%), Other (13%), Bamboo (7%), TeamCity (4%), Circle CI (3%), Travis CI (10%), None (10%)
  - **How many times do you commit code to CI/CD build per day**: 1 time (22%), 2 times (16%), 3 times (18%), 4 times (9%), 5 and more times (35%)
  - **Percent of GC algorithms**:
    - Java 10 and before: SerialGC (22%), ParallelGC (19%), G1 (22%), CMC (21%)
    - Java 11 and after: G1 (68%), SerialGC (33%), CMC (4%), ParallelGC (1%)
  - **Database**: PostgreSQL (34.4%), MySQL (26.9%), Elasticsearch (18.3%), Oracle (18.3%), MSSQL (14%), IBM DB2 (12.9%), MariaDB (12.9%), MongoDB (7.5%), None (6.5%), DynamoDB (4.3%), Other (4.3%), SQLLite (2.2%), Couchbase (1.1%), Firebase (1.1%)
- **Spring Boot 3**
  - Spring Boot 3 runs on Java 17 (which is the minimum version required) and supports records.
  - New Micrometer for metrics and tracing, Spring Cloud Sleuth project becomes obsolete.
  - Java EE is no longer used in favor of Jakarta EE, which means no longer `javax` packages but the `jakarta` ones.
  - Spring Security 6 has a major change where `SecurityChainFilter` has to be used instead of `WebSecurityConfigurerAdapter`.
  - Spring Data JPA and Hibernate 6
  - AOT GraalWM support for native images making Spring Native obsolete as it was an experimental project, not it is supported out-of-the box.
- **Java 18**
  - Multiline String, Switch Expressions, Records, Pattern Matching for `instanceof`, better NPE error messages, faster start-up and lower memory footprint

### Impression ⭐⭐☆☆☆
- ✅ A nice and brief overview of the new and incoming technologies and upgrades as well as an overview of the usage statistics from various sources.
- ⛔ Though it is nice to know which JRE/JDK distribution the speaker prefers, no technical reasoning was provided instead. It's nice to know what offers a "killer feature", but what exactly it is? Next time less of hype, swag, and buzzwords, but more explanation.

_____

## Scalable backend
- (in original: Škálovatelný backend)

> "An universal truth about architecture does not exist and its design must be context-aware."
- Length 1:00:39, watched on 2021-11-12, **#architecture #monolithic**
- Roman Bouchner
- Language: Czech 🇨🇿

### Keynotes
- Though it is a modern conception to have multiple instances, it's required to know the main goals:
  - No downtime deployment, resiliency against HW failure, better performance (huge amount of users) and its protection on high traffic.  
- Scaling doesn't mean to increase a number of nodes, but mind the CPU and RAM memory as databases are resources demaning. Though, scaling assures high availability (HA).
- Worth to read: https://spoilerproxy.com/ and https://goodbackend.com/.
- **Context**: Small development team (also DevOps and testing), fast paced product, strong focus on data consistency, simple architecture, infrastructure and code, simple error codes and their handling.
- **Rules**: Backend are stateless and all states are in the database (including the locking), backends don't call each other (how to handle 504 timeout?).
- **Idea**: Producer-consumer architecture (the BE manages data from the FE, sneds to a queue and the BE workers process them), the resutls processed in 3 seconds are returned synchronously, otherwise an information about an upcoming notification is offered.
- **Solution**: 
  - Scalable monolithic architecture deploying the very same configurable JAR (favors easy development) thorugh properties `api.enabled=true` and `worker.threads=1` and more layers as the properties switch if the JAR will serve as a Worker or the API REST (Main) service.
  - In case the Main service decides it's going to take a lot of time, the request is sent into a queue from where Workers take and process them.
  - **Queue**: The queue is implemented by PostgreSQL database as it assures the transactional manner, data consistency and simple backups (Kafka is rather suitable for non-transactional data, for example email notifications). The database is a single source of truth.
    - 1 record is represented by exactly one row (important).
    - Data: RequestId (for Kibana), UserRequestContext (user identification, JSON request), WorkerId, RequestParameters, State (Waiting -> Processing -> Done/Error -> ErrorResolved), Result, Error message.
    - `INSERT` into the database is easy, but `SELECT` cannot get everything as long as synchronization between the workers is required so the record is processed by exactly one worker only:
    ```sql
    BEGIN
    SELECT * FROM my_queue WHERE state='waiting' FOR UPDATE SKIP LOCKED LIMIT 1
    UPDATE my_queue SET state='processing' WHERE id = ...
    COMMIT;
    ```
  - The stored JSON request assures that the request can be processed by a Worker regardless of its origin as it follows a defined format.  
  - **Polling? Notifications?**: The problem was how often to poll the requests from the queue? Once a second or 10 seconds?
    - The neat solution is to notify other backends without actually calling them -> PostgeSQL notifications.
    - The PostgreSQL notifications are an in-built solution that and transactional and easy to use.
    ```bash
    pgsql NOTIFY <channel> <payload>
    pgsql LISTEN <channel>
    ```
    This can be implemented into Java by a custom implementation:
    ```java
    pgListenerService.notify("worker", "params");
    pgListenerService.addServiceListener("worker", params -> { });
    ```
  - **Database scaling for HA**: The main goal is the high availability (HA), the idea behind is that the more dumb the database is, the easier it can be scaled. 
    - PostgreSQL is capable of having one primary database for read and write and a secondary one for reading only. Internally it uses WAL (Write-Ahead Logging) and phisical transaction replication. Theoretically, the data can be available for read with a tiny delay in terms of miliseconds, but it is useful for analytical and aggregation processing. 
    - In
  - **Database scaling for multiple users**: Another goal is to avoid distributed databases as the development gets complex as well as its testing.
    - The solution is to add more databases but in the way a transactional communication is **never** required between them.
    - A proper sharding implementation should assure that the relevant data always stay together in a single database (one company data are only in a single databasase). With a new big customer new cloud (shard), but the same architecture and software can be used.
    - It is required to implement a switch (here is possible to use Kafka, RabbitMQ as long as the consistency is not what matters here, but a quick switching).
    - It is also recommend to use UUID to distinguish company data for easy migration across the shardes.
  - **Database migration**: It is not easy to rename columns or tables and it must happen in multiple steps as long as multiple versions of the application can use the same database schema.
  - **Error handling**: There is no sophisticated error handling required as no retries are implemented, the record just fails. If a problem persists for a longer time, it's worth to take a look at it.

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
- Spring Boot Maven Plugin is simple to use, the command `mvn spring-boot:build-image` downloads a builder image where the application is built and the result is a Docker image (it is required to has Docker installed and Docker daemon run) - the result image is **layered**. It is required to include the plugin:
  ```xml
  <plugin>
      <groupId>org.springframework.boot</groupId>
      <artifactId>spring-boot-maven-plugin</artifactId>
  </plugin>
  ```
  
  There is Bellsoft Liberica JDK inside out-of-the-box for unknown reason, though there are better JDK distributions.
- **Layered image**
  - Example from infrequently to frequently changed parts: `spring-boot-loader`, `dependencies`, `snapshot-dependencies`, `application`
  - Layers enable only the changed parts can be replaced: in case we change the `dependencies`, then at least the `spring-boot-loader` can remain same. If we change the `application` part, only the `application` part is sent to Docker registry or Kubernetes nodes.
  - Layered JARs, images work with JIB or Builpacks and saves the time between build and deployment (network traffic between Jenkins, Kubernetes nodes etc.)
- **OpenJ9 Buildpack**: Buildpacks can be browset at: https://github.com/orgs/paketo-buildpacks/repositories?q=jre
  - Configuration is in the `spring-boot-maven-plugin`
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
  - The application build happens in the builder image, there are 3 builders out-of-the-box: `full`, `base` and `tiny`. They differ in the amount of libraries installed, though the most used one is `tiny`. It is possible to create an own builder, though it is really complicated and worth only for corporates where the implementation of such a builder must be certified security-wise. Jib also allows to crate a custom builder in a simpler way.
    ```xml
    <configuration>
      <image>
        <name>TODO_IMAGE_NAME</name>
        <buildpacks>
          <builder>paketobuildpacks/builder:tiny</buildpack>
        </buildpacks>
      </image>
    </configuration>
    ```
  - The plugin also can push into Docker registry:
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
    ```bash
    mvn -Ddocker.username=TODO -Ddocker.password=TODO spring-boot:build-imaage
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
  ```bash
  mvn spring-boot:build-image -Pnative
  ```
  Paketo buildpacks have also CLI that can build the native images:
  ```bash
  pack build test_img --builder=paketobuildpacks/builder:base -e BP_JVM_VERSION=17
  ``` 
- **Alternatives**
  - It is still possible to write Dockerfiles (a great tutorial is at spring.io/guides/topicals/spring-boot-docker)
  - As long as we are not ready for buildpacks, Jib is a good choice as it is really easy to use (`maven jib:build`) and a subsequent transition to buildpacks is not hard. We can also use Jib without Spring Boot.
  - JLink is **not** a good alternative because it conflicts the layered JARs concepts, as long as each application has own JRE, so they cannot share the same layers. 
- **Goals (regardless of the technology)**: Layered images, smaller images, CI/CD image builds, distroless images
  - Distroless images are without Linux distribution and contain only the application, though there is no `bash` to use in the container, it is smaller and safe from attacks.

### Impression ⭐⭐⭐⭐⭐
- ✅ Detailed and comprehensible overview of how to build Docker images using buildpacks. Jib mentioned and offered as a simple alternative.
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
  - Other: File structure, Declaration and usages...
- **Opening and reading**:
  - Multicolumn edit (Mouse Middle button, or **⌥⌘⇧** and left click and drag).
  - Multiple carets (**⌥⇧** and click)
  - Quick open understands wildcard (**⇧⇧** and type `*Controller`).
  - Other: Mnemonic bookmarks, Find in the previous search (for example: `pet` AND `@Entity`).
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
  - Key promoter to suggest shortcuts for repetitive actions
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
> "The entire JVM was reworked to support the virtual theads."
- Length 43:11, watched on 2021-11-12, **#java #multithreading**
- Miroslav Sevelda
- Language: Czech 🇨🇿

### Keynotes
- History:
  - Java 1 - Basic support for multithreading
  - Java 5 - Thread pools, executor services, futures, callable
  - Java 7 - Fork/join framework (velmi důležitý pro virt. vláken jako scheduler pro mapování na fyzická)
  - Java 8 - Completable futures, lambda, streams
  - Java 9 - Reactive streams (against IO bound threads)
  - Java 19 - Virtual threads
- **Current model**: In the current model, a thread in the JVM always means there is a corresponding OS thread linked. This model will be still available and unchanged with the Project Loom. 
- **Project Loom** ([JEP 425](https://openjdk.org/jeps/425)): Brings a new solution of massive parallelism and introduces virtual threads that are invisible from the point of view of the OS. It means it's possible to create teoretically billion of threads without saturating the OS. This principle is similar to what Python uses: virtual thread synchronization into a single one. This project doesn't introduce virtual threads only.
- Motto: Easy-to-use, hight-throughput, leightweight concurrency and new programming models.
- **Virtual thread** is planned and manager thread visible only on the JVM level and is similar to the [green thread](https://en.wikipedia.org/wiki/Green_thread) concept and analogous to the currently unused POSIX threads.
  - The solution was to return back to the M:N model: In this case the JVM platform thread is mapped to the OS thread and a huge amount of virtual threads. Context switch through a scheduler mounts the virtual thread to the JVM platform thread, which is a single OS thread.
  - **Terminology**:
    - Virtual thread: - Invisible in the OS.
    - Platform thread: - JVM thread mapped to the OS thread.
    - Carried thread - Platform thread bound to the virtual thread as it is not possible to run a virtual thread with no platform thread. 
    - Thread mounting - Process when the virtual thread is assigned to the platform one.
    - Thread unmounting - Process when the virtual thread is unassigned from the plarform one. It happens automatically as soon as the virtual thread invokes a blocking operation.
  - **Disadvantages of the current model**:
    - JVM thread is bound to the OS thread, which means the thread management is above the JVM and thread creation is expensive. 
    - Inflexible memory allocation for the thread stack memory, which is not under control of the JVM.
    - Problematic support for massive parallelism and not optimal for IO-bound threads that are not computing in a blocked state.
  - **Advantages of the new model**:
    - Virtual threads are inexpensive, so it's possible to create billion of virtual threads, basically as much as we need without the OS and resources limits.
    - Scheduling and the memory management is under the JVM control and the GC.
    - Alternative to the Async-IO and reactive approaches.
    - No dangerous operations like suspending or stopping threads since the virtual threads are un/mounted automatically.
  - **Disadvantages of the new model**:
    - The debugging caan become harder as it is no longer possible to use the debugging tools on the OS level.
    - It is too soon for comprehensible conclusions. 
- **New API**: Only few changes were introduced for minimal interference to the existing API for sake of easy transition to virtual threads. The new solution completes the current API design and the virtual thread is still an instance of `Thread` as well as the platform thread.
  - Each virtual thread is of a type `DAEMON` and has fixed `NORM_PRIORITY` that cannot be changed (as it never worked correctly and synchronization primitives was always a better way to go).
  - The virtual thread scheduling is implemented with the existing `ForkJoinPool` in the FIFO mode that implements the "work stealing", though it is partially customizable and it is possible to use a custom scheduler (but why). It's great virtual threads are built on the existing and well-known implementation.
  - **New factory methods**: The old implementation is unchanged and it is needed to use factory methods to create a virtual thread.
    - `Thread vt = Thread.ofVirtual()` - creates a virtual thread
    - `Thread pt = Thread.ofPlatform()` - creates a platform thread
    - `Thread vt = Thread.startVirtualThread()` - creates and starts a virtual thread
  - **Fluent style**:
    - `Thread vt = Thread.ofVirtual().name("virtual").unstarted(runnable);
    - `Thread vt = Thread.ofPlatform().name("platform").unstarted(runnable);
  - **Builder and factory styles**
  - **Methods**:
    - `boolean isPlatformVirtual = Thread.ofPlatform().isVirtual(); // false`
    - `boolean isVirtualVirtual = Thread.virtual().isVirtual(); // true`
    - `boolean isVirtualDaemon = Thread.virtual().isDaemon(); // true`
  - **Executor services**:
    - `ExecutorService service = Executors.newVirtualThreadPerTaskExecutor();`
- **Antipatterns**
  - The virtual threads should not bee pooled as long as they are lightweight and the pool management becomes an overheads compared to threads creations. However, there is a new dedicated thread pool `ExecutorService`, though it's better to just create a thread and let the system to handle it.
  - Do not use priorities with virtual threads.

### Impression ⭐⭐⭐⭐⭐
- ✅ I don't know if I am impressed by the speaker or the topic. Disadvantages and patterns were well-explained. 
- ⛔ None about the session. I think I can give up on Project Reactor and Spring Webflux.

_____

## Domain Driven Microservices
> "The used language should be ubiquitous."
- Length 49:24, watched on 2021-11-12, **#domain #analysis**
- Ivan Macalák
- Language: Czech 🇨🇿

### Keynotes
- Domain Driven Design is an approach to software development that helps us to break down a compex system into loosely coupled components with well-encapsulated logic and clearly defined dependencies among them. 
- It's needed to have a *strategy* that matches the architecture.
- **Domain** is a sphere of knowledge representad by the *ubiquitous language* and encapsulates a domain model and bounded context.
  - The *ubiquitous language* is important as analyst and developer should use same language and same terms.
  - **Bounded context** enables decomposing to smaller parts, for example Smart building managemnt:
    - Building management -> Occupant (Name, Floor, Flat number, Relations).
    - User profile -> User (Name, Favourites, Contacts, Payment methods, Invoice address).
    - Incident management -> Reporter (Name, Email, Phone)
    - Authorization -> User (Username, Email, Password, Roles)
  - **Domain vision statement** 
  - TODO

### Impression ⭐⭐⭐☆☆
- ✅ A necessity of an ubiquitous language is highlighted. The session clearly demonstrated how the Domain Diven Design is coupled with Microservice Architecture.
- ⛔ Too theoretical and abstract, it would be nice to show a sample core, generic and supporting domain designed in detail.

_____

## Don't be scared of benchmarks in development
- (in original: Nebojte se benchmarků při vývoji)
> "Moore's Law ceases to apply as a single core performance converges to a limit defined by the laws of physics."
- Length 45:53, watched on 2021-11-13, **#java #jmh #benchmarks**
- Jan Novotný
- Language: Czech 🇨🇿

### Keynotes
- Moore's Law ceases to apply as a single core performance converges to a limit defined by the laws of physics: Performance becomes a thing again!
  - The producers compensate the performance limits by adding more threads.
- **Java Microbenchmark Harness (JMH)** is a low-lever test framework for simple and quick *unit* and *integration* performance tests writing.
  - Maven dependencies: `org.openjdk.jmh:jmh-core` (`compile`) and `org.openjdk.jmh:jmh-generator-annprocess` (`provided`).
  - Samples are available at https://github.com/openjdk/jmh/tree/master/jmh-samples/src/main/java/org/openjdk/jmh/samples 
  - There are three basic ways to run it:
    - Using IntelliJ Idea using a JMH plugin (click to the green triangle and run as a test).
    - Using a main class:
    ```java
    org.openjdk.jmh.Main.main(args);
    ```
    - Using the command line, for which it's necessary too use a Maven Shade Plugin (`org.apache.maven.plugins:maven-shade-plugin`) to create a fat jar (also called *uberjar*) that contains the performance tests.
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
    ```bash
    java -jar target/benchmarks.jar
    ```
  - **Configuration**
    - **Annotations** are available to configure the test, though they can be overriden with the command line arguments.
      - `@Benchmark` annotates the performance test itself.
      - `@Warmup` defines the warm-up.
      - `@Measurement` defines the benchmark measurement details.
      - `@Fork` defines the forking. The test should run in the separate JVM (`@Fork(1)`) to not influent the tests and yield representative results
      - `@BenchmarkMode` and `@OutputTimeUnit` to define the output.
      - `@Setup(Level.XXX)` and `@TearDown(Level.XXX)` for test and data preparations.
      - `@State(Scope.XXX)` to define te test data scope.
    - **Builder** using `OptionsBuilder` contains a context help thanks to it's fluent style and using `include(String regex)` can define through CI/CD what set of tests would be run, assuming smart package naming.
  - **Lifecycle of the test**
    - There are three levels: `Level.Trial`, `Level.Iteration`, and `Level.Invocation`.
      - **Trial** is run *once* before (`@Setup(Level.Trial`) and after (`@TearDown(Level.Trial`) the test and is used for initialization and closing resources.
      - **Iteration** is run *always* before (`@Setup(Level.Iteration`) and after (`@TearDown(Level.Iteration`) each test iteration and is used for the data preparation and clean-up.
      - **Invocation** is run *always* before (`@Setup(Level.Invocation`) and after (`@TearDown(Level.Invocation`) the test method (`@Benchmark`) itself and might possibly have impact to the test, so it's recommended to not handle data in this phase, unless it's quick compared to the test execution itself.
  - **Data preparation**
    - A stateful data object annotated with `@State` and defined scope is passed as a formal parameter to the method annotated with `@Benchmark`.
    - **Scopes** define the liveness of the `@State` data object:
      - `Scope.Thread` is the most used one and the data are isolated and instantiated per thread.
      - `Scope.Benchmark` creates one instance for all the tests and threads, so beware the synchronization and access.
      - `Scope.Group` grants all instances will be shared across all threads within the same group defined by `@Group`. This advanced scope is the least and the hardest to use and configure correctly.
  - **Debugging**
    - The debugging of the test (especially data preparation) does not work with a JVM fork (`@Fork(1)`). For this purpose, the fork has to be disabled (`@Fork(0)`).  
  - **Gotchas**
    - It's needed to watch out the data if they are sent with each iteration as we assume.
    - Constant folding: The compiler eliminates useless code and pre-calculates predictable results. It's needed ot use a return type or `Blackhole` (can be used as a formal parameter to the `@Benchmark` method) to consume the result.
    - Safe-looping: The compiler elimineates useless iterations and does magic with cycles at all (unrolling, jamming, vectorization), so it's better to leave the iteration mechanisms to the JMH and measure only the algorithm itself.
  - **Profiles** reveal the reasoning behind the bad test results as we want to know why.
    - IntelliJ idea has an own profiler displaying the process and time diagram of test method execution.
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
    - Ask the following: What I try to measure? Do I measure it correctly? Why the result is not I expect? What happens?
    - Do not get stick with the absolute numbers and rather compare and use the relative numbers as the results depend on hardware, OS, surrounding code, etc.
    - Use the production-alike data.
    - Observe the `BLOCKED` thread time in multithreading applications.
    - Be careful with formulating and summarizing the results. It's worth to consult with a colleague, review the test and involve more people.
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
  - It's not possible to allocate a new instance of an object, because the memory run out in the Heap.
  - A huge array is allocated that doesn't fit in the memory.
  - Native memory ran out in the Metaspace.
  - Allocation of memory failed on native code call through JNI
  - High overhead of Garbage Collector (GC)
    - By default, if Garbage Collector takes 98% or more of the JVM run and deallocates less than 5% of memory, the error is thrown
  - It's not possible to create a new thread, because the underlying OS limits for the maximum number of threads (this surprisingly throws this error as JVM has not much information from the OS).
- **Cases when `java.lang.StackOverflowError` occurs**:
  - Excessive deep or infinite recursion.
- **JVM memory management**:
  - **Heap**: Object allocation, array allocation, String pool, GC
    - The Heap is divided to 2 basic sections: Young Generation (Eden + Survival) and Old Generation
    - The GC checks the younger objects more often than the survival and old ones.
    - Most of the problems are related to Heap and Non-Heap: Although the overall memory allocated of the Heap is sufficient,`java.lang.OutOfMemoryError` is thrown when a single section gets full. For example, it doesn't matter the remaing sections are nearly empty if the Eden section is full. 
  - **Non-Heap**: Internal data used by the JVM that are invisible to a developer (code cache, formerly Permanent Generation (PermGen), now Metaspace).
  - **Stack**: There are 2 types of stack: Native Stack (for native and JNI methods) and a Normal Stack (for our methods). Each thread has own stack.
    - Method calls and metadata storage. Each *frame* has: Return value, local variables, operand stack, current class constant pool reference (into the Non-Heap memory).
- **Garbage Collector (GC)**
  - The Heap memory is hierarchically divided by young/old generation and furhter sub-groups for optimized and fairly sophisticated run.
  - General garbage collecting algorithms overview:
    - **Tracing (Reachability tree): The GC traverses the oriented graph of objects, traces for the reachable ones and removes the unreachable ones. Though this algorithm is slow and expensive, but can detect and remove cyclical references. JVM GC uses this algorithm.
    - **Reference counting**: Counts the number of references and removes if fall into zero. This algorithm can miss cyclical references.
  - By default, the less memory is available, the more aggressively the GC runs to release the memory in the JVM. This approach delays  `java.lang.OutOfMemoryError`, though the overhead of the GC run raises and the application becomes less responsive (lags).
- **String internization** is implemented using the flyweight design pattern (referencing to a shared copy).
  - String literals (those between `""`) are interned (pooled) automatically. Though we can call `String#intern`, it's not recommended for the short-lived strings as we risk wasting the memory.
  - It's also not a good idea to intern the sensitive data as it's not under our control when they are removed from the memory by the GC. For this reason, all sensitive content should be passed through `char []`.
- **Java 8 changes to the JVM**
  - Permanent Generation is replaced by more dynamic Metaspace. It caused problems with multiple hot-deploy (ex. Tomcat, etc.) when the JVM is not registerd. Though a new classloader is loaded and the reference to the old one is discarded and the class references become replaced by the new one, but releasing of the the long-living classes takes a delay (if they are released at all) and the maximum memory limit can be hit. 
  - **Permanent Generation (PermGen)** has a fixed size of a allocated continuous block of native memory in the OS that is **not** efficiently deallocated.
    - `-XX:PermSize=[size]` and `-XX:MaxPermSize=[size]` parameters.
  - **Metaspace** has a dynamically allocated memory continuous block of native memory in the OS that is efficiently deallocated as long as the OS only limits of how much memory is can be provided.
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
    - Minimize stateful integration and HTTP sessions usage.
    - Make the application stateless.
    - Beware of soft/weak references in cache and the keys size (it is not a good idea to put a whole request as a key).
  - A large number of hash-based structures (`HashMap` and `HashSet`) is also not a good idea and a plain array can be a better choice.
  - VisualVM is a nice tool but favors smaller Heap sized.

### Impression ⭐⭐⭐⭐☆
- ✅ Educative session about how is JVM memory management done in a sufficient detail.
- ⛔ I expected more of "tips and tricks", especially ineffective code snippets and how to fix them.

_____

## Experience with Spring native
- (in original: Zkušenosti se Spring Native)
> "Nobody uses Liferay and WAS today."
- Length 42:55, watched on 2021-11-13, **#spring #native #graalvm**
- Jiří Pinkas
- Language: Czech 🇨🇿

## Keynotes
- Spring Boot 3 is in its final design as Spring Native for Spring Boot 2 was rather experimental, vastly different from Spring Boot 3, and the entire implementation for native support and  ahead-of-time (AOT) was 3 times reworked. GraalVM Native Support needs to be included in [start.spring.io](https://start.spring.io/).
- **GraalVM native image**
  - A technology that compiles ahead-of-time Java code into a standalone runnable application called a *native image*.
  - Such an application contains application classes, dependency classes and classes used by Java runtime and native JVM code.
  - Native images don't run on JVM (but they come from JVM), but they load important JVM components like memory management, thread scheduling, etc. from a differnt runtime called Subtrate VM.
  - The result application has a quick start (doesn't load classpath and classes that happens now on the build time), and consumes less of RAM compared to JVM.
  - Process: Java bytecode (application, dependencies, JVM) → Native image build (static analysis finds what is used, initialization, snapshot) → Binary code (code, image heap).
  - Use cases:
    - Microservices - resulting Docker image is smaller, starts-up quickly and has lower memory footprint
    - Serverless and CLI applications - they start instantly
  - GraalVM community version uses only the old SerialGC that is suitable only for smaller heaps, though GraalVM enterprise edition can use G1.
- **Native and dynamic code**
  - What is saved into a native image depends on the result of the static analysis on the native image build time. 
  - Such an analysis **can't** find out the usages of JNI, reflections, dynamic proxies or resources from classpath - such classes need to be added manually through configurations. Luckily, Spring can do that.
    ```    
    META-INF/
    ├─ native-image/
    │  ├─ resource-congif.json
    │  ├─ serialization-config.json
    │  ├─ jni-config.json
    │  ├─ proxy-config.json
    │  ├─ reflect-config.json
    ```
  - This was a huge problem since Spring Framework is built on top of reflections and dynamic proxies. The creators had to catch up with Micronaut and Quarkus and implement the native images support. They originally ignored benefits of a quick start-up, then they found out that serverless is an interesting use-case and finally, they found out they are fucked up. The implementation of AOT was lengthy and reworked 3 times. 
  - GraalVM can't dynamically create runtime classes out-of-the box.
- **Spring Boot 3**
  - It's required to have GraalVM installed as a SDK to support GraalVM.
  - The exectution of `mvn clean spring-boot:build-image -Pnative` calls `spring-boot-maven-plugin:process-aot` itnernally that runs a Spring container and discovers what beans were created on the application load and generates the following:
    - `graalvm-reachability-metadata`: `reflct-config.json`, `resource-config.json`, etc. from various libraries
    - `spring-aot`: `reflect-config.json`, `resource-config.json` from the application
  - Spring luckily doesn't need to store all beans into such JSON configuration files, but only their definitions.
  - For example: Spring Data JPA beans are normally created on the application startup, now it's not possible so that's why the AOT plugin was created.
  - The creators of Spring AOT found out that such an approach can be used even for non-Spring applications, so it makes sense as a slight performance and size improvement, although the native would not be used. 
- **Native executable** is no longer platform-agnostic, which is completely different from what Java was created on top of. Now the solution brings a platform-specific executable, which is ok, beacuse we have Docker and CI/CD that were not available years ago. We somehow reinvented the old solution. 
- **Comparison** (the more points, the better):
  |                    | JVM | Native | Remark                                                                        |
  |--------------------|-----|--------|-------------------------------------------------------------------------------|
  | Maturity           | 100 | 50     | JVM is a proven solution, native is pretty much new                           |
  | Build time         | 10  | 2      | What is 5 seconds for JVM becomes tens of minutes for native                  |
  | Startup time       | 20  | 100    | What is seconds and minutes for JVM is miliseconds for native                 |
  | Latency/throughput | 100 | 7      | JIT in a long run can optimize the runtime, which is not possible for native. |
  | Memory footprint   | 50  | 100    | What is 200 MB RAM for JVM becomes 50 MB RAM for native                       |
  - Build time becomes very lengthy and it is not possible to reduce it significantly.
  - Image size is smaller for native solutions, but custom layered images are useless for native solutions, because each image has a custom and optimized JDK for a given applicaiton.
  - Memory footprint is also smaller for native solutions.
- **Problems**:
  - How to register resources, proxy classes or classes used by reflection? A solution is to implement `RuntimeHintsRegistrar` and activate with `@ImportRuntimeHints`: 
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
    classes.forEach(clazz -> reflectionHints.registerType(class, categories));
    ```
- **Production support**:
  - [GraalVM Dashboard](https://www.graalvm.org/dashboard/) can introspect the contents of the built application.
  - [Dive](https://github.com/wagoodman/dive) can instrospect layered Docker images.
  - Actuator metrics becomes limited as they don't display used memory amount. 
  - Profiling becomes problematic and Java Flight Recorder limited.
  - **Heap size tuning**:
    - `docker run -m 200m --rm -it -p 8080.8080 <image_name> -XX:+PrintGC -XX:+VerboseGC` prints each GC run details. Currently there is no other solution.
  - **Observation** of a sample stateless application:
    - RAM was reduced from 200 MB to 50 MD, response time got lowered from 60ms to 30ms, start-up took only 70ms.
    - The build time increased brutally from few seconds to 3-6 minutes.
- **Future**:
  - Native image support to be standardized in OpenJDK through Project Leyden
  - Reachability metadata repository is a repository of reflection and dynamic proxies for various projects so we would write and configure JSON configurations as least as possible. GraalVM thoroughly cooperates with Spring.
    - Link: https://medium.com/graalvm/enhancing-3rd-party-library-support-in-graalvm-native-image-with-shared-metadata-9eeae1651da4

### Impression ⭐⭐⭐⭐⭐
- ✅ Excellent understanding and experience of the speaker as well as his ability to explain simmply and highlight the important aspects of the native approach. Solution to common problems.
- ⛔ -

_____

## Web Services, SOAP, REST and how to design them
- (in original: Web Services, SOAP, REST aneb jak je správně navrhovat)
> "Insurance companies have contracts older than 30 years that need to be supported, though the products are no longer offered. For that reason they use old systems."
- Length 52:14, watched on 2021-11-13, **#rest #soap**
- Petr Adámek
- Language: Czech 🇨🇿

## Keynotes
- The author has experience with rather older projects as he works as a consultant for corporates.
- Law of the instrument (law of the hammer, Maslow's hammer): Is a cognitive bias that involves an over-reliance on a familiar tool: "I hold a hammer, everithing becomes a nail".
- There is not an universal solution and tools, there exist limits and exceptions, and quite often.
- **SOAP vs REST**:
  |                  | SOAP                                  | REST                                            |
  |------------------|---------------------------------------|-------------------------------------------------|
  | Characteristics  | Heawyweight                           | Lightweight                                     |
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
  - Due to the historical reason. The other party requires it.
    - Insurance companies have contracts older than 30 years that need to be supported, though the products are no longer offered. For that reason they use old systems. It makes no sense for such companies to rewrite the existing solutions that become deprecated with time. Also the XML structures tend to be rich and complex in definition and XML allows nesting.
  - It's needed to build something on top of the existing SOAP solution. It's needed to route through multiple nodes (SOAP is protocol independent). 
  - It's needed ot use XML, WSDL or SOAP extensions (WS-security, WS-MeliableMessaging, WS-Addressing) or use it as an universal format.
  - Reasons XML is required: There is an existing schema to be used. Produce SOAP as a REST service. Schemes need to be combined. There is a need for semistructured data. There is a need for XSLT transformations.
- **Best practices**:
  - Contract first as it's possible to develop in parallel, unless a small BE-FE application with few endpoints is developed.
  - Well-defined contract including the non-standard situations and error codes. An empirical approach about how the service works is not a good idea.
  - Use standard and appropriate error codes for a particular situation (4XX and 5XX for the beginning). 
  - Think out-of-the-box and don't let the Law of the instrument to influent you, for example there are other solutions aside from REST and SOAP:
    - GraphQL
    - Messaging (JMS, Kafka, RabbitMQ etc.)
  - Client identification and correlation ID
  - REST API versioning with backward-compatibility: The approach with headers is not usually recommended and it's better to include the version to the path which is handy for the future version decomissioning.
  - REST API filter: If there is required a sophisticated fitler for nested projection, better grab GraphQL.

### Impression ⭐⭐⭐⭐⭐
- ✅ A great speech proving SOAP is not dead (ex. insurance industry), though shall rather not be used for the greenfield projects. Well-explained comparison focusing on *when* SOAP or REST shall be used and how, instead of just a shallow comparison.
- ⛔ I would expect some design tips and tricks for SOAP as I know REST quite well.

_____

## GraalVM: Java ♥ Python ♥ Micronaut
> "It's possible to render beautiful graphs with `pygal` in Java through GraalVM."
- Length 44:33, watched on 2021-11-13, **#graalvm #java #python #polygot**
- Štepán Šindelář
- Language: Czech 🇨🇿

## Keynotes

- **GraalVM** is an universal virtual machine for running application written in JavaScript, Python, Ruby, R, JVM-based languages (Java, Kotlin, Scala) and LLVM-based languages (C, C++). It is similar to JVM that supports native images, JIT mode, non-JVM languages - a kind of universal swiss knife.
  - The structure is very similar to the standard JVM, but has additional tools:
    - `./bin/gu` - `gu` is a tool for installing and managing optional GraalVM language runtimes and utilities, that can be listed with `./bin/gu list`, for example `./bin/gu install python` installs the Python language runtime
    - `./bin/graalpy` starts the Python CLI
- **GraalPy** only supports currently Max/Linux, but is compatible with CPython. Unlike JPython supports native extensions, such as NumPy, Matplotlib, etc. The peak performance in on par with PyPy (currently the fastest alternative). It also supports Java interoperability and Python venv.
- It is possible to call Python code from Java as well as Python scripts, though GraalVM doesn't support multiple return types from Python to Java.
- The GraalVM can be included to the IDE as a SDK and the GraalVM-specific classes are already a part of the SDK, so the IDE should recognise them without importing a Maven dependency. 
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
  - Simple and quick scripting where Python excels primarly (though alternatives are to write a Maven plugin or dependency), but this is useful for smaller companies.
  - To render beautiful graphs with `pygal` in Java through GraalVM.  
  
### Impression ⭐⭐⭐⭐⭐
- ✅ Though I am not interested in Python, the capabilities of GraalVM are fucking lit. The live coding done well.
- ⛔ -
