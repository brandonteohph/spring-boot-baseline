# Java Baseline Debugging

## Introduction

This is a **Spring Boot baseline for microservices**.

The project serves as a minimal foundation for building, debugging, and experimenting with Java-based microservices using Spring Boot. It is intentionally lightweight so additional capabilities such as logging, messaging, concurrency, and integrations can be added incrementally.

---

## Java and Spring Boot Version

- Java Version: 21  
- Spring Boot Version: 4.0.3  

---

## Dependencies and Plugins

| Dependency Name | Type (Dependency/Plugin) | Version | Purpose |
|-----------------|-------------------------|---------|---------|
| spring-boot-starter-webmvc | Dependency | inherited (Spring Boot 4.0.3) | Provides Spring MVC framework for building REST APIs |
| spring-boot-starter-webmvc-test | Dependency | inherited (Spring Boot 4.0.3) | Provides testing utilities for Spring MVC applications |
| spring-boot-maven-plugin | Plugin | inherited (Spring Boot 4.0.3) | Packages and runs the Spring Boot application |

---

## Run Steps

### 1. Install Java

Install Java 21 from official sources:

- https://jdk.java.net/  
- https://adoptium.net/  

Verify installation:

```bash
java -version
```

Set JAVA_HOME if required:

```bash
export JAVA_HOME=/path/to/jdk-21
export PATH=$JAVA_HOME/bin:$PATH
```

---

### 2. Run the Application

```bash
./mvnw spring-boot:run
```

---

### 3. Build the Application

```bash
./mvnw clean package
```

Output will be in:

```text
target/
```

---

## Notes

This repository is intended as a baseline and can be extended with:

- structured logging
- external API integrations
- Kafka or messaging systems
- asynchronous processing
- thread pool configuration
- containerisation
- observability and metrics
