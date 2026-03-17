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

### Dependencies

- spring-boot-starter-webmvc (compile): Provides Spring MVC framework for building REST APIs
- spring-boot-starter-webmvc-test (test): Provides testing utilities for Spring MVC applications

### Plugins

- spring-boot-maven-plugin (version inherited from parent): Packages and runs the Spring Boot application

---

## Run Steps

### 1. Install Java

Install Java 21 from:

- https://jdk.java.net/
- https://adoptium.net/

Verify installation:

java -version

Set JAVA_HOME if required:

export JAVA_HOME=/path/to/jdk-21
export PATH=$JAVA_HOME/bin:$PATH

---

### 2. Run the Application

./mvnw spring-boot:run

---

### 3. Build the Application

./mvnw clean package

Output will be in:

target/

---

## Notes

This repository is intended as a baseline and can be extended with logging, messaging, concurrency, and observability features.
