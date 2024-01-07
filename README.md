# microservices-circuit-breakers
 <br>
Spring Cloud Gateway is a project built on top of Spring WebFlux and Project Reactor to provide an API gateway and a central place to handle cross-cutting concerns like security, resilience, and monitoring.<br>
The Polar Bookshop system needs an edge server to route traffic to the internal APIs and address several cross-cutting concerns.<br>
These are the main dependencies:<br>
Spring Cloud Gateway (org.springframework.cloud:spring-cloud-starter-gateway)—Provides utilities to route requests to APIs and cross-cutting concerns like resilience, security, and monitoring. It’s built on top of the Spring reactive stack.<br>
Spring Boot Test (org.springframework.boot:spring-boot-starter-test)—Provides several libraries and utilities for testing applications, including Spring Test, JUnit, AssertJ, and Mockito. It’s automatically included in every Spring Boot project.<br>
<br>
Spring Cloud Gateway provides three main building blocks:<br>
Route—This is identified by a unique ID, a collection of predicates for deciding whether to follow the route, a URI for forwarding the request if the predicates allow, and a collection of filters that are applied either before or after forwarding the request downstream.<br>
Predicate—This matches anything from the HTTP request, including path, host, headers, query parameters, cookies, and body.<br>
Filter—This modifies an HTTP request or response before or after forwarding the request to the downstream service.<br>
