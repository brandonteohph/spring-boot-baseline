# Java Baseline Debugging

## Introduction

This project provides a **Spring Boot baseline for microservices**.

The repository is intended as a foundation for building and debugging Java microservices using Spring Boot. It is designed to act as a lightweight environment for experimenting with service architecture, runtime behaviour, and integration patterns.

Typical uses for this baseline include:

- experimenting with Spring Boot configuration
- testing microservice architecture patterns
- debugging application startup and runtime behaviour
- building integrations with external APIs or messaging systems
- exploring Java concurrency and multithreading

This project is intentionally minimal so that additional infrastructure (logging, messaging, API integrations, concurrency patterns, etc.) can be layered in incrementally.

---

## Plugins

The following Maven plugins are applied in this branch.


| Plugin                   | Purpose                                       |
| -------------------------- | ----------------------------------------------- |
| spring-boot-maven-plugin | Packages and runs the Spring Boot application |

### spring-boot-maven-plugin

This plugin allows the project to:

- run the application directly using Maven
- package the application as an executable JAR
- support Spring Boot’s dependency and packaging conventions

Official documentation:

https://docs.spring.io/spring-boot/docs/current/maven-plugin/reference/html/

---

## Run Steps

### 1. Install Java

This project requires **Java (JDK)** to run.

Recommended version: **Java 21 (LTS)** or newer.

Official sources:

OpenJDK builds
https://jdk.java.net/

Eclipse Temurin builds
https://adoptium.net/

After installation verify Java is available:

```bash
java -version
```

You should see output similar to:

```bash
openjdk version "21"
```

If necessary, configure the JAVA_HOME environment variable.

Example for Linux/macOS:

```bash
export JAVA_HOME=/path/to/jdk
export PATH=$JAVA_HOME/bin:$PATH
```

### 2. Run the Application

This project includes the Maven Wrapper, so installing Maven manually is not required.

From the project root run:

```bash
./mvnw spring-boot:run
```

The application will start using the embedded Spring Boot server.

### 3. Build the Application

To compile and package the application:

```bash
./mvnw clean package
```

The generated artifact will appear in:

```bash
target/
Project Structure
src
 ├─ main
 │  ├─ java
 │  └─ resources
 └─ test
```

## Notes

This repository is designed as a baseline microservice foundation and can be expanded with additional capabilities such as:

- structured logging
- external API integrations
- Kafka or messaging systems
- asynchronous processing
- thread pool configuration
- containerisation
- observability and metrics
