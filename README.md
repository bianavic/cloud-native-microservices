# cloud native microservices studies

### objective
What Cloud-Native microservices are, and how we can easily build with Spring Cloud.

### book
Hands On Microservices with Kotlin
- chapter 6 Creating Cloud-Native Microservices

### Spring Cloud Architecture

#### Configuration server:
- provides the capability to be queried about configurations, so when a microservice starts, it can retrieve all the 
values that need to be configured, such as URL, database connections, password, and anything that can be configured, from the Configuration Server

#### Service discovery: Eureka
- we use service discovery service to register or find instances of our microservice
obs: Heart-beat mechanism: a way for a microservice to tell a Service Discovery that it is available and ready to work

#### Load Balancer pattern: Ribbon
-  choose instances available among them to perform our request. this make an optimal usage of the instances, and split the load among them evenly.

#### Gateway pattern: Zuul
- is an entry point to our microservice, we expose them using a simple route and manage the details for them
obs: can also be used as the entry point to our security

#### Circuit breaker: Hystrix
- it's a way to deal with operations that can eventually fail. it has an open or closed status, telling us if the operation 
that encapsulates can be used—think of circuit breakers as fuses in an electrical installation.



