# Spring-Cloud
Spring Boot + Spring Cloud + Eureka + Feign

## Boot Start
Enable Cluster Eureka Servers, Achieve high availabilities
> `cd spring-cloud-server`

> `mvn clean package`

> `java -jar spring-cloud-server-0.0.1-SNAPSHOT.jar spring.profiles.active=s1`

> `java -jar spring-cloud-server-0.0.1-SNAPSHOT.jar spring.profiles.active=s2`

Visit `http://localhost:8761` or `http://localhost:8762`

Run SpringCloudClientApp, revisit `http://localhost:8761`, a message indicating a client has set up will show up

* s1 and s2 here correspond to the names of the application.yml files, syntax is spring.profiles.active=xxx
* These jar packages can be run on several servers later on

