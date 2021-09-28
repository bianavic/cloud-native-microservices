# Configuration Server

A Configuration Server allows us to serve any microservice the configuration that it may need, so when a microservice starts, it will require no more configurations than just the one from where the Configuration Service is located.

When a microservice starts, it can retrieve all the values that need to be configured, such as URL, database connections, password, and anything that can be configured, from the Configuration Server

### tools ####

- Maven
- Kotlin
- Spring Boot: Config Server, Eureka Server

- IntelliJ

obs: Cipher data with Java Cryptography

### port ###

server.port = 8888

### production profile ###

``
$ ./mvnw package

$ java -jar target/config-server-0.0.1-SNAPSHOT.jar --spring.cloud.config.profile=production

```