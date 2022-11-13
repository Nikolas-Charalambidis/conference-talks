# [JavaDays 2022](https://www.javadays.cz/en/)

- Czech Republic 🇨🇿, Prague, CineStar Černý Most
- November 2022
- Both onsite and online
- The conference is paid and the online access is granted for a limited time (1-2 weeks).

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
- TODO

### Impression ⭐⭐⭐☆☆
- ✅ 
- ⛔ Too theoretical, it would be nice to show a sample core, generic and supporting domain designed in detail.

_____

## Don't be scared of benchmarks in development
- (in original: Nebojte se benchmarků při vývoji)
> ""
- Length 45:53, watched on 2021-11-13, **#java #jmh #benchmarks**
- Jan Novotný
- Language: Czech 🇨🇿

_____

## Tips and tricks for Java memory management
- (in original: Tipy a triky práce s pamětí v Javě)
> ""
- Length 48:54, watched on 2021-11-13, **#java #jvm #gc #memory**
- Petr Adámek
- Language: Czech 🇨🇿

_____

## Experience with Spring native
- (in original: Zkušenosti se Spring Native)
> ""
- Length 42:55, watched on 2021-11-13, **#spring #native #graalvm**
- Jiří Pinkas
- Language: Czech 🇨🇿

_____

## Web Services, SOAP, REST and how to design them
- (in original: Web Services, SOAP, REST aneb jak je správně navrhovat)
> ""
- Length 52:14, watched on 2021-11-13, **#rest #soap**
- Petr Adámek
- Language: Czech 🇨🇿

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
