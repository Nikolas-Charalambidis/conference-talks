# [Spring One](https://springone.io/)

- All sessions for free and online since the 7th of September 2021

## [How To Be a Java Automated Testing Superstar](https://springone.io/2021/sessions/how-to-be-a-java-automated-testing-superstar)
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
- ✅ Very catchy speech, theoretical aspects and importance of testing, best-practices of unit testing
- ⛔ Too short (not the speaker's fault), code examples weren't that impressive, no mention about [BDD](https://en.wikipedia.org/wiki/Behavior-driven_development) approach

## [Deploy Code into Production Faster on Kubernetes](https://springone.io/2021/sessions/modern-application-configuration-in-kubernetes)
- Length 27:31, watched on 2021-09-07, **#devops #kubernetes #cloud #native**
- Valentina Alaria as Director Product Management, VMware
- Track: Cloud Native Platforms

### Keynotes
- Most of Kubernetes offerings are delivered as a bag of parts
  - 63 % of organizations, if use K8S, use as internal platforms or build internal platforms
  - 94 % of organizations, if use K8S, building internal platforms use more than one platform
  - 58 % of organizations agree that architectural decision making has gotten harder
- Developer experience on DIY platforms is lacking. Developers must still maintain containers, configure containers run through multiple layers of YAML, manage IT and security aspects
- Importance lies in tooling to help developers: leverage automatized DevOps practices,  enforce organizational best-practices, app-aware platform

### Rating ⭐⭐☆☆☆
- ✅ Beginner-friendly introduction, developer concerns identification
- ⛔ The structure doesn't match the agenda in the introduction, chaotic jumping between topics, rather Tanzu platform promotion, lacking expected pure K8S tips

